

- Create ML
- MLImageClassifier
- MLImageClassifier.ModelParameters
-  init(validation:maxIterations:augmentation:algorithm:) 

Initializer

# init(validation:maxIterations:augmentation:algorithm:)

Creates model training parameters.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+visionOS 1.0+

``` source
init(
    validation: MLImageClassifier.ModelParameters.ValidationData = __Defaults.validation,
    maxIterations: Int = __Defaults.maximumIterations,
    augmentation: MLImageClassifier.ImageAugmentationOptions,
    algorithm: MLImageClassifier.ModelParameters.ModelAlgorithmType = __Defaults.algorithm
)
```

## Parameters 

`validation`  

Labeled data that the model evaluates on for validation. The default is `.split(strategy: .automatic)`.

`maxIterations`  

The maximum number of training iterations to use during training. The default is 25.

`augmentation`  

The image augmentation options to use to increase the training data variety. If no data augmentation needs to be applied, use `[]` as input. Otherwise, inputs take the form `[.crop, .blur]`.

`algorithm`  

The type of model algorithm to use for training. The default is a logistic regression classifier with a `sceneprint(revision: 1)` feature extractor.

## See Also

### Creating parameters

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

enum ModelAlgorithmType

The model algorithm to use for training an image classifier.

