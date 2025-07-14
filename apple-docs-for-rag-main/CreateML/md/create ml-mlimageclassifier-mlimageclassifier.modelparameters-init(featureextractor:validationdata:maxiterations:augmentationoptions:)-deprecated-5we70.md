

- Create ML
- MLImageClassifier
- MLImageClassifier.ModelParameters
-  init(featureExtractor:validationData:maxIterations:augmentationOptions:) Deprecated

Initializer

# init(featureExtractor:validationData:maxIterations:augmentationOptions:)

Creates a new set of image classifier parameters with validation data represented by a dictionary.

iOS 15.0–16.0DeprecatediPadOS 15.0–16.0DeprecatedMac Catalyst 15.0–16.0DeprecatedmacOS 10.14–10.15DeprecatedvisionOS 1.0+

``` source
init(
    featureExtractor: MLImageClassifier.FeatureExtractorType = .scenePrint(revision: 1),
    validationData: [String : [URL]]?,
    maxIterations: Int = 25,
    augmentationOptions: MLImageClassifier.ImageAugmentationOptions = []
)
```

Deprecated

Use the validation property instead.

## Parameters 

`featureExtractor`  

A versioned feature extractor.

`validationData`  

Validation data represented by a dictionary.

`maxIterations`  

The maximum number of training iterations to use during training. The default is 25.

`augmentationOptions`  

The image augmentation options to use to increase the training data variety.

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

enum ClassifierType

Type of classifier to be used.

enum ModelAlgorithmType

The model algorithm to use for training an image classifier.

