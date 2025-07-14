

- Create ML
- MLImageClassifier
- MLImageClassifier.ModelParameters
-  augmentationOptions 

Instance Property

# augmentationOptions

The variations the training session uses to generate more variety in the training dataset.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+visionOS 1.0+

``` source
var augmentationOptions: MLImageClassifier.ImageAugmentationOptions
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

var maxIterations: Int

The maximum number of iterations the training session can use.

var validationData: [String : [URL]]?

A set of images that the training process uses for validation.

Deprecated

