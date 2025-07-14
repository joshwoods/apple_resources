

- Create ML
- MLImageClassifier
-  MLImageClassifier.ModelParameters 

Structure

# MLImageClassifier.ModelParameters

Parameters that affect the process of training an image classifier model.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+visionOS 1.0+

``` source
struct ModelParameters
```

## Overview

Use this structure to configure the model training session. With it you can:

- Set a limit to the number of training iterations the session can use

- Provide your own validation dataset. See MLImageClassifier.ModelParameters.ValidationData.

- Enable specific image augmentations. See MLImageClassifier.ImageAugmentationOptions.

- Designate a custom feature extractor. See MLImageClassifier.FeatureExtractorType.custom(_:).

Once you configure an MLImageClassifier.ModelParameters instance, use it to configure a training session with one of the applicable MLImageClassifier asynchronous type methods or synchronous initializers.

## Topics

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

enum ModelAlgorithmType

The model algorithm to use for training an image classifier.

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

var validationData: [String : [URL]]?

A set of images that the training process uses for validation.

Deprecated

### Describing parameters

var description: String

A text representation of the model parameters.

var debugDescription: String

A text representation of the model parameters that’s suitable for output during debugging.

var playgroundDescription: Any

A description of the model parameters shown in a playground.

### Supporting types

enum FeatureExtractorType

The underlying base model that extracts image features for image classifier training session.

enum ValidationData

The source of a validation dataset for an image classifier.

struct ImageAugmentationOptions

The variations that the training process can use to generate more training data from the training data you provide.

### Default Implementations

CustomDebugStringConvertible Implementations

CustomPlaygroundDisplayConvertible Implementations

CustomStringConvertible Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomPlaygroundDisplayConvertible
- CustomStringConvertible

## See Also

### Related Documentation

static func train(trainingData: MLActionClassifier.DataSource, parameters: MLActionClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLActionClassifier>

Begins an asynchronous action classifier training session.

init(trainingData: MLImageClassifier.DataSource, parameters: MLImageClassifier.ModelParameters) throws

Creates an image classifier with a training dataset represented by a data source.

init(trainingData: [String : [URL]], parameters: MLImageClassifier.ModelParameters) throws

Creates an image classifier with a training dataset represented by a dictionary.

Deprecated

### Supporting types

enum DataSource

A data source for an image classifier.

