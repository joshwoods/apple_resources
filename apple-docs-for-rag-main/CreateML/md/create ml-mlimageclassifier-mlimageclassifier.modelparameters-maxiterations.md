

- Create ML
- MLImageClassifier
- MLImageClassifier.ModelParameters
-  maxIterations 

Instance Property

# maxIterations

The maximum number of iterations the training session can use.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+visionOS 1.0+

``` source
var maxIterations: Int
```

## See Also

### Accessing the training parameters

var algorithm: MLImageClassifier.ModelParameters.ModelAlgorithmType

Model algorithm to be used

var featureExtractor: MLImageClassifier.FeatureExtractorType

The underlying base model the training session uses to extract image features as it trains an image classifier.

Deprecated

var validation: MLImageClassifier.ModelParameters.ValidationData

The image classifier’s validation dataset.

var augmentationOptions: MLImageClassifier.ImageAugmentationOptions

The variations the training session uses to generate more variety in the training dataset.

var validationData: [String : [URL]]?

A set of images that the training process uses for validation.

Deprecated

