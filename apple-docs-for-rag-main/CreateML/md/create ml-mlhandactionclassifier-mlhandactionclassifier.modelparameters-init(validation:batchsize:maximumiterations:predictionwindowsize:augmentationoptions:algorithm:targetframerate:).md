

- Create ML
- MLHandActionClassifier
- MLHandActionClassifier.ModelParameters
-  init(validation:batchSize:maximumIterations:predictionWindowSize:augmentationOptions:algorithm:targetFrameRate:) 

Initializer

# init(validation:batchSize:maximumIterations:predictionWindowSize:augmentationOptions:algorithm:targetFrameRate:)

Creates a set of training session parameters for a hand action classifier task.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
init(
    validation: MLHandActionClassifier.ModelParameters.ValidationData = .split(strategy: .automatic),
    batchSize: Int = MLHandActionClassifier.__Defaults.batchSize,
    maximumIterations: Int = MLHandActionClassifier.__Defaults.maximumIterations,
    predictionWindowSize: Int = MLHandActionClassifier.__Defaults.predictionWindowSize,
    augmentationOptions: MLHandActionClassifier.VideoAugmentationOptions = [],
    algorithm: MLHandActionClassifier.ModelParameters.ModelAlgorithmType = .gcn,
    targetFrameRate: Double = MLHandActionClassifier.__Defaults.targetFrameRate
)
```

## Discussion

- validation: An MLHandActionClassifier.ModelParameters.ValidationData instance.

- batchSize: The number of videos the training session uses for each of its training iterations.

- maximumIterations: The largest number of training iterations the training session can use.

- predictionWindowSize: The number of frames the training session uses to train a hand action classifier. For example, set to 60 to capture hand actions that take 2 seconds from videos that have a frame rate of 30 frames per second.

- augmentationOptions: The variations the training session uses to add more variety to its training dataset.

- algorithm: The algorithm the training session uses to train the hand action classifier.

- targetFrameRate: The number of frames the training session uses per second of video to train a hand action classifier.

