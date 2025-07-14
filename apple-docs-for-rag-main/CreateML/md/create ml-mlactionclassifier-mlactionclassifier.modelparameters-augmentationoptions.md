

- Create ML
- MLActionClassifier
- MLActionClassifier.ModelParameters
-  augmentationOptions 

Instance Property

# augmentationOptions

The variations the training session uses to generate more variety in the training dataset.

macOS 11.0+

``` source
var augmentationOptions: MLActionClassifier.VideoAugmentationOptions
```

## See Also

### Accessing the training parameters

var maximumIterations: Int

The largest number of training iterations the training session can use.

var batchSize: Int

The number of videos the training session uses for each of its training iterations.

var targetFrameRate: Double

The number of frames the training session uses per second of video to train an action classifier.

var predictionWindowSize: Int

The number of frames the training session uses to train an action classifier.

var algorithm: MLActionClassifier.ModelParameters.ModelAlgorithmType

The algorithm the training session uses to train the action classifier.

var validation: MLActionClassifier.ModelParameters.ValidationData

The action classifier’s validation dataset.

