

- Create ML
- MLImageClassifier
- MLImageClassifier.ModelParameters
-  MLImageClassifier.ModelParameters.ClassifierType 

Enumeration

# MLImageClassifier.ModelParameters.ClassifierType

Type of classifier to be used.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+visionOS 1.0+

``` source
enum ClassifierType
```

## Topics

### Designating an algorithm’s classifier

case logisticRegressor

Logistic regression is a statistical model that classifies input feature vector into different categories.

case multilayerPerceptron(layerSizes: [Int])

Multilayer perceptron, layerSizes holds a list of positive integers that represent the number of hidden units in each layer. An additional fully connected layer with a Softmax activation output will be added that maps to probabilities of sound categories.

### Describing a classifier type

var description: String

A textual representation of this instance.

### Operators

static func == (MLImageClassifier.ModelParameters.ClassifierType, MLImageClassifier.ModelParameters.ClassifierType) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- CustomStringConvertible
- Equatable
- Hashable
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

enum ModelAlgorithmType

The model algorithm to use for training an image classifier.

