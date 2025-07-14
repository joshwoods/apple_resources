

- Create ML
- MLImageClassifier
- MLImageClassifier.ModelParameters
-  MLImageClassifier.ModelParameters.ModelAlgorithmType 

Enumeration

# MLImageClassifier.ModelParameters.ModelAlgorithmType

The model algorithm to use for training an image classifier.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+visionOS 1.0+

``` source
enum ModelAlgorithmType
```

## Topics

### Designating an algorithm type

case transferLearning(featureExtractor: MLImageClassifier.FeatureExtractorType, classifier: MLImageClassifier.ModelParameters.ClassifierType)

Train using a transfer-learning algorithm with a specified feature extractor and classifier.

### Describing an algorithm type

var description: String

A textual representation of this instance.

## Relationships

### Conforms To

- CustomStringConvertible
- Sendable

## See Also

### Creating parameters

init(validation: MLImageClassifier.ModelParameters.ValidationData, maxIterations: Int, augmentation: MLImageClassifier.ImageAugmentationOptions, algorithm: MLImageClassifier.ModelParameters.ModelAlgorithmType)

Creates model training parameters.

init(featureExtractor: MLImageClassifier.FeatureExtractorType, validation: MLImageClassifier.ModelParameters.ValidationData, maxIterations: Int, augmentationOptions: MLImageClassifier.ImageAugmentationOptions)

Creates a new set of training parameters for an image classifier with a validation dataset.

Deprecated

init(featureExtractor: MLImageClassifier.FeatureExtractorType, validationData: MLImageClassifier.DataSource, maxIterations: Int, augmentationOptions: MLImageClassifier.ImageAugmentationOptions)

Creates a new set of image classifier parameters with validation data represented by a data source.

Deprecated

init(featureExtractor: MLImageClassifier.FeatureExtractorType, validationData: [String : [URL]]?, maxIterations: Int, augmentationOptions: MLImageClassifier.ImageAugmentationOptions)

Creates a new set of image classifier parameters with validation data represented by a dictionary.

Deprecated

enum ClassifierType

Type of classifier to be used.

