

- Create ML
- MLHandPoseClassifier
- MLHandPoseClassifier.ModelParameters
-  maximumIterations 

Instance Property

# maximumIterations

The largest number of training iterations you allow the training session to use.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
var maximumIterations: Int
```

## See Also

### Accessing hand pose training parameters

var batchSize: Int

The number of images the model training session uses for each training iteration.

var algorithm: MLHandPoseClassifier.ModelParameters.ModelAlgorithmType

The algorithm the training session uses to create the hand pose classifier.

var augmentationOptions: MLHandPoseClassifier.ImageAugmentationOptions

The variations the training session uses to add more variety to its training dataset.

var validation: MLHandPoseClassifier.ModelParameters.ValidationData

A dataset the hand pose classifier task uses to evaluate the model that’s distinct from the training dataset.

