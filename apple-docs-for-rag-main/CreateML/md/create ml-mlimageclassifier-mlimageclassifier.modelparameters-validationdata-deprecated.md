

- Create ML
- MLImageClassifier
- MLImageClassifier.ModelParameters
-  validationData Deprecated

Instance Property

# validationData

A set of images that the training process uses for validation.

iOS 15.0–16.0DeprecatediPadOS 15.0–16.0DeprecatedMac Catalyst 15.0–16.0DeprecatedmacOS 10.14–10.15DeprecatedvisionOS 1.0+

``` source
var validationData: [String : [URL]]? { get set }
```

Deprecated

Use the validation property instead.

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

var augmentationOptions: MLImageClassifier.ImageAugmentationOptions

The variations the training session uses to generate more variety in the training dataset.

