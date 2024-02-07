# NLP projects

Including parser, word2vec model, and machine translation modules as well. 


* Emotion Detection in Speech modifies existing codebase to identify emotions from spoken language. 
## Analyzing audio signals
![IMG_5924](https://github.com/rhea-mal/semantics/assets/70975260/5fec2faf-5d78-4d3b-9f83-8937cf7a228d)

### Datasets:
The foundation of this model is built on two datasets:
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


## Model Development
The project explored various neural network architectures, with Convolutional Neural Networks (CNN) providing the best performance. Model refinement focused on achieving a balance between complexity and accuracy, ultimately reaching just over 70% validation accuracy. Model evaluation was conducted through comparisons of predicted vs. actual emotions on test data. Further validation involved live testing with newly recorded voices expressing various emotions, demonstrating the model's effectiveness in real-world scenarios.
