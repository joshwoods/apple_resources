

- Create ML
- MLImageClassifier
- MLImageClassifier.ModelParameters
-  featureExtractor Deprecated

Instance Property

# featureExtractor

The underlying base model the training session uses to extract image features as it trains an image classifier.

iOS 15.0–16.0DeprecatediPadOS 15.0–16.0DeprecatedMac Catalyst 15.0–16.0DeprecatedmacOS 10.14–11.0DeprecatedvisionOS 1.0+

``` source
var featureExtractor: MLImageClassifier.FeatureExtractorType { get set }
```

Deprecated

Use featureExtractor in ModelAlgorithmType instead.

## Discussion

When you train an image classifier with Create ML, you don’t train a complete model that converts images to labels. Instead, Create ML leverages a *feature extractor*, which is another model that identifies a set of general but distinguishing image characteristics. You can either use Create ML’s `scenePrint` feature extractor or provide your own custom feature extractor.

In either case, you train your model to map the feature extractor’s output to labels in a process known as *transfer learning*. Your model effectively borrows the knowledge of the feature extractor to accelerate its own training process while requiring fewer training images.

## See Also

### Accessing the training parameters

var algorithm: MLImageClassifier.ModelParameters.ModelAlgorithmType

Model algorithm to be used

var validation: MLImageClassifier.ModelParameters.ValidationData

The image classifier’s validation dataset.

var maxIterations: Int

The maximum number of iterations the training session can use.

var augmentationOptions: MLImageClassifier.ImageAugmentationOptions

The variations the training session uses to generate more variety in the training dataset.

var validationData: [String : [URL]]?

A set of images that the training process uses for validation.

Deprecated

