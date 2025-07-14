

- Create ML
- MLImageClassifier
- MLImageClassifier.ModelParameters
-  init(featureExtractor:validation:maxIterations:augmentationOptions:) Deprecated

Initializer

# init(featureExtractor:validation:maxIterations:augmentationOptions:)

Creates a new set of training parameters for an image classifier with a validation dataset.

iOS 15.0–16.0DeprecatediPadOS 15.0–16.0DeprecatedMac Catalyst 15.0–16.0DeprecatedmacOS 10.15–11.0DeprecatedvisionOS 1.0+

``` source
init(
    featureExtractor: MLImageClassifier.FeatureExtractorType = .scenePrint(revision: 1),
    validation: MLImageClassifier.ModelParameters.ValidationData = .split(strategy: .automatic),
    maxIterations: Int = 25,
    augmentationOptions: MLImageClassifier.ImageAugmentationOptions = []
)
```

Deprecated

Use featureExtractor in ModelAlgorithm Type instead.

## Parameters 

`featureExtractor`  

The feature extractor you want Create ML to use during the training session.

`validation`  

A validation dataset.

`maxIterations`  

The maximum number of training iterations to use during training. The default is 25.

`augmentationOptions`  

The image augmentation options to use to increase the training data variety.

## See Also

### Creating parameters

init(validation: MLImageClassifier.ModelParameters.ValidationData, maxIterations: Int, augmentation: MLImageClassifier.ImageAugmentationOptions, algorithm: MLImageClassifier.ModelParameters.ModelAlgorithmType)

Creates model training parameters.

init(featureExtractor: MLImageClassifier.FeatureExtractorType, validationData: MLImageClassifier.DataSource, maxIterations: Int, augmentationOptions: MLImageClassifier.ImageAugmentationOptions)

Creates a new set of image classifier parameters with validation data represented by a data source.

Deprecated

init(featureExtractor: MLImageClassifier.FeatureExtractorType, validationData: [String : [URL]]?, maxIterations: Int, augmentationOptions: MLImageClassifier.ImageAugmentationOptions)

Creates a new set of image classifier parameters with validation data represented by a dictionary.

Deprecated

enum ClassifierType

Type of classifier to be used.

enum ModelAlgorithmType

The model algorithm to use for training an image classifier.

