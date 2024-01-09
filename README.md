SPEECH EMOTION RECOGNITION WITH AUDIO FEATURE EXTRACTION

Speech Emotion Recognition is a field of study that involves the identification and analysis of emotional states conveyed through speech. It aims to capture the emotional content of spoken language, allowing machines to understand and respond to human emotions.

Understanding human emotions in speech is essential for developing more empathetic and responsive human-computer interaction systems as well as for applications in customer service, virtual assistants, mental health monitoring, and more. It enables systems to adapt their responses based on the emotional context, thereby enhancing user experience.

In this project, I have explored Speech Emotion Recognition using machine learning techniques. 

I’ve used the RAVDESS dataset (acronym for the Ryerson Audio-Visual Database of Emotional Speech and Song) which comprises of 7,356 files, each rated by 247 individuals on emotional validity, intensity, and genuineness through 10 evaluations.

The project utilizes audio feature extraction to analyze and identify emotions in speech, focusing on anger, calmness, fear and happiness.

Libraries used:

1) Librosa: Librosa is a Python library for music and audio analysis. In this project, it is used for audio processing and feature extraction, specifically for extracting Mel-frequency cepstral coefficients (MFCC), chroma features, and mel spectrogram features from the audio files.

2) Soundfile: Soundfile is used for reading sound files, providing functionalities to read and process audio files.

3) NumPy: NumPy is a fundamental package for scientific computing with Python. It is utilized for numerical operations on the extracted audio features.

4) Scikit-learn: Scikit-learn provides machine learning tools. The MLPClassifier from scikit-learn is employed for training a Multi-layer Perceptron (MLP) model for emotion classification. It also offers utilities for model evaluation, such as accuracy score, classification report, and confusion matrix.

Process Steps:

a) Data Collection: Audio data from various actors is collected, each labeled with an emotion. We have skipped this step since we are using an already available dataset with labelled audio files.

b) Feature Extraction: Librosa is used to extract relevant audio features, including MFCC, chroma, and mel spectrogram.

c) Data Preprocessing: The dataset is preprocessed to filter out emotions not in the target list. In this project, we have considered four emotions – anger, calmness, fear and happiness.

d) Data Splitting: The dataset is split into training and testing sets.

e) Model Training: An MLP classifier is trained on the training set.

f) Model Evaluation: The trained model is evaluated on the test set using accuracy, classification report, and confusion matrix.

- MFCCs capture the spectral characteristics of audio signals.
The code calculates the mean of the MFCCs for each audio file, capturing the average spectral characteristics. These coefficients serve as essential features for characterizing the nuances of speech.

- Chroma features provide information about the harmonic content of audio signals.
The mean of the chroma features is computed in the code, contributing valuable information about the musical aspects of the speech, particularly useful for emotional tone recognition.

- Mel spectrogram features capture the frequency content of audio signals across time. 
The mean of the mel spectrogram features is computed, providing insights into the frequency content over time – which provides a comprehensive characterization of the emotional nuances present in the speech signal.

- The MLPClassifier in scikit-learn is a Multi-layer Perceptron, a type of neural network used for supervised learning tasks. It learns by adjusting its settings based on examples, using a method called backpropagation and pays attention to complex patterns in the input data using activation functions.


Applications of Speech Emotion Recognition:

- Speech Emotion Recognition enhances Human-Computer Interaction (HCI) by enabling systems to discern and respond to users’ emotional states conveyed through speech. 

- SER can be applied to tailor user interfaces, virtual assistants, and customer service interactions based on detected emotions, which fosters more personalized and empathetic responses. 

- In educational software, SER can adapt learning environments to suit students’ emotional engagement, while in healthcare, it can aid in mental health monitoring. Entertainment platforms can leverage SER to dynamically adjust content and accessibility options to benefit individuals with special needs. Overall, SER enriches HCI, creating emotionally intelligent systems that enhance user experience across various domains.


Future Scope:

The model can be improved by incorporating a more diverse dataset with varied accents, languages, and emotional expressions. It can also be improved with continuous learning strategies to adapt to evolving speech patterns and expressions. 

 
