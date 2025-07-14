

- Create ML
- MLSoundClassifier
- MLSoundClassifier.ModelParameters
- MLSoundClassifier.ModelParameters.ModelAlgorithmType
-  MLSoundClassifier.ModelParameters.ModelAlgorithmType.transferLearning(featureExtractor:classifier:) 

Case

# MLSoundClassifier.ModelParameters.ModelAlgorithmType.transferLearning(featureExtractor:classifier:)

An algorithm that leverages the knowledge of a general-purpose model built into the operating system.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+visionOS 1.0+

``` source
case transferLearning(
    featureExtractor: MLSoundClassifier.ModelParameters.FeatureExtractorType,
    classifier: MLSoundClassifier.ModelParameters.ClassifierType
)
```

## Parameters 

`featureExtractor`  

The extractor type the algorithm uses to detect features from the audio data.

`classifier`  

The model type the algorithm uses to classify audio data.

## Discussion

You typically use this transfer-learning algorithm to train an object detector in these situations:

- Your training dataset has a limited number of examples.

- You prefer your object detector’s Core ML model file to be as small as possible.

## See Also

### Designating an algorithm

enum FeatureExtractorType

The feature-extractor options for a sound-classifier training algorithm.

enum ClassifierType

The classifier options for a sound classifier training algorithm.

