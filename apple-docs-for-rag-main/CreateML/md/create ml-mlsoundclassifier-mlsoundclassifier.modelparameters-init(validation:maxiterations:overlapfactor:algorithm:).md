

- Create ML
- MLSoundClassifier
- MLSoundClassifier.ModelParameters
-  init(validation:maxIterations:overlapFactor:algorithm:) 

Initializer

# init(validation:maxIterations:overlapFactor:algorithm:)

Creates a new set of training parameters for a sound classifier with a validation dataset and a training algorithm.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+visionOS 1.0+

``` source
init(
    validation: MLSoundClassifier.ModelParameters.ValidationData = __Defaults.validation,
    maxIterations: Int = __Defaults.maximumIterations,
    overlapFactor: Double = __Defaults.overlapFactor,
    algorithm: MLSoundClassifier.ModelParameters.ModelAlgorithmType = __Defaults.algorithm
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

`algorithm`  

The algorithm the training session uses to train the sound classifier.

## See Also

### Creating parameters

init(validation: MLSoundClassifier.ModelParameters.ValidationData, maxIterations: Int, overlapFactor: Double)

Creates a new set of training parameters for a sound classifier with a validation dataset.

init(validation: MLSoundClassifier.ModelParameters.ValidationData, maxIterations: Int, overlapFactor: Double, algorithm: MLSoundClassifier.ModelParameters.ModelAlgorithmType, featureExtractionTimeWindowSize: TimeInterval)

Creates a new set of training parameters for a sound classifier with a validation dataset, a training algorithm, and a time-window size.

