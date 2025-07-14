

- Create ML
- MLImageClassifier
- MLImageClassifier.ModelParameters
-  validation 

Instance Property

# validation

The image classifier’s validation dataset.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+visionOS 1.0+

``` source
var validation: MLImageClassifier.ModelParameters.ValidationData { get set }
```

## See Also

### Accessing the training parameters

var algorithm: MLImageClassifier.ModelParameters.ModelAlgorithmType

Model algorithm to be used

var featureExtractor: MLImageClassifier.FeatureExtractorType

The underlying base model the training session uses to extract image features as it trains an image classifier.

Deprecated

var maxIterations: Int

The maximum number of iterations the training session can use.

var augmentationOptions: MLImageClassifier.ImageAugmentationOptions

The variations the training session uses to generate more variety in the training dataset.

var validationData: [String : [URL]]?

A set of images that the training process uses for validation.

Deprecated

