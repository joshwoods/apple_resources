

- Create ML
- MLSoundClassifier
- MLSoundClassifier.ModelParameters
-  init(validation:maxIterations:overlapFactor:) 

Initializer

# init(validation:maxIterations:overlapFactor:)

Creates a new set of training parameters for a sound classifier with a validation dataset.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+visionOS 1.0+

``` source
init(
    validation: MLSoundClassifier.ModelParameters.ValidationData = .split(strategy: .automatic),
    maxIterations: Int = 25,
    overlapFactor: Double = 0.5
)
```

## Parameters 

`validation`  

A validation dataset represented by an MLSoundClassifier.ModelParameters.ValidationData instance.

`maxIterations`  

The largest number of iterations the training session can use to train the sound classifier.

`overlapFactor`  

A proportion of overlap the training session uses to analyze two consecutive windows in the audio data. The proportion must be in the range `[0.0, 1.0)`. Higher proportions generate more training data, but also increases the training time.

The default value is `0.5`, which represents a 50% overlap.

## See Also

### Creating parameters

init(validation: MLSoundClassifier.ModelParameters.ValidationData, maxIterations: Int, overlapFactor: Double, algorithm: MLSoundClassifier.ModelParameters.ModelAlgorithmType)

Creates a new set of training parameters for a sound classifier with a validation dataset and a training algorithm.

init(validation: MLSoundClassifier.ModelParameters.ValidationData, maxIterations: Int, overlapFactor: Double, algorithm: MLSoundClassifier.ModelParameters.ModelAlgorithmType, featureExtractionTimeWindowSize: TimeInterval)

Creates a new set of training parameters for a sound classifier with a validation dataset, a training algorithm, and a time-window size.

