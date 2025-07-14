

- Create ML
- MLHandActionClassifier
- MLHandActionClassifier.ModelParameters
-  algorithm 

Instance Property

# algorithm

The algorithm the training session uses to create the hand action classifier.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
var algorithm: MLHandActionClassifier.ModelParameters.ModelAlgorithmType
```

## See Also

### Accessing hand action training parameters

var maximumIterations: Int

The largest number of training iterations you allow the training session to use.

var batchSize: Int

The number of videos the model training session uses for each training iteration.

var targetFrameRate: Double

The number of video frames per second the hand action classifier model expects as its input at runtime.

var predictionWindowSize: Int

The number of video frames the model training session uses to train a hand action classifier.

var augmentationOptions: MLHandActionClassifier.VideoAugmentationOptions

The variations the training session uses to add more variety to its training dataset.

var validation: MLHandActionClassifier.ModelParameters.ValidationData

A dataset the hand action classifier task uses to evaluate the model that’s distinct from the training dataset.

