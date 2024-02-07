# Emotion Detection in Speech


* The Emotion Detection in Speech project aims to develop a machine learning model capable of identifying emotions from spoken language. In an era where personalization enhances daily experiences, the potential applications of such technology are vast. Industries ranging from marketing to automotive can leverage emotion detection to tailor services, such as personalized advertising or adjusting autonomous vehicle behavior for safety.

## Analyzing audio signals
![](images/joomla_speech_prosody.png?raw=true)

[©Fabien_Ringeval_PhD_Thesis](https://drive.google.com/file/d/0B2V_I9XKBODhcEtZV1lRWW1fYTg/view).
<br>

### Datasets:
The foundation of our model is built on two key datasets:
1. [RAVDESS](https://zenodo.org/record/1188976).
RAVDESS: A collection of 1500 audio recordings from 24 actors (12 male and 12 female), expressing 8 distinct emotions. Each file's naming convention includes a specific character indicating the emotion conveyed.
2. [SAVEE](http://kahlan.eps.surrey.ac.uk/savee/Download.html).
SAVEE: Comprising about 500 recordings by 4 male actors, this dataset labels emotions through the initial characters of each file name.

## Audio files:
Analytical Techniques
Audio Analysis
Initial analyses involved plotting waveforms and spectrograms of the audio files to understand their characteristics.

Feature Extraction
Using the LibROSA library, features were extracted from the audio to facilitate model learning. Key steps included timing each file to 3 seconds for uniformity and doubling the sampling rate to enrich the feature set.
![feature](https://github.com/rhea-mal/semantics/assets/70975260/917de25f-5dad-438a-8ec5-7ba8e9d9694d)


## Models

Model Development
The project explored various neural network architectures, with Convolutional Neural Networks (CNN) providing the best performance. Model refinement focused on achieving a balance between complexity and accuracy, ultimately reaching just over 70% validation accuracy.

Evaluation and Predictions
Model evaluation was conducted through comparisons of predicted vs. actual emotions on test data. Further validation involved live testing with newly recorded voices expressing various emotions, demonstrating the model's effectiveness in real-world scenarios.
