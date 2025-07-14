

- Create ML
- MLHandPoseClassifier
- MLHandPoseClassifier.ModelParameters
-  init(validation:batchSize:maximumIterations:augmentationOptions:algorithm:) 

Initializer

# init(validation:batchSize:maximumIterations:augmentationOptions:algorithm:)

Creates a set of training session parameters for a hand pose classifier task.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
init(
    validation: MLHandPoseClassifier.ModelParameters.ValidationData = .split(strategy: .automatic),
    batchSize: Int = MLHandPoseClassifier.__Defaults.batchSize,
    maximumIterations: Int = MLHandPoseClassifier.__Defaults.maximumIterations,
    augmentationOptions: MLHandPoseClassifier.ImageAugmentationOptions = [],
    algorithm: MLHandPoseClassifier.ModelParameters.ModelAlgorithmType = .gcn
)
```

## Discussion

- validation: An MLHandPoseClassifier.ModelParameters.ValidationData instance.

- batchSize: The number of images the training session uses for each of its training iterations.

- maximumIterations: The largest number of training iterations the training session can use.

- augmentationOptions: The variations the training session uses to add more variety to its training dataset.

- algorithm: The algorithm the training session uses to train the hand pose classifier.

