

- Create ML
- MLImageClassifier
- MLImageClassifier.ModelParameters
-  MLImageClassifier.ModelParameters.ValidationData 

Enumeration

# MLImageClassifier.ModelParameters.ValidationData

The source of a validation dataset for an image classifier.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+visionOS 1.0+

``` source
enum ValidationData
```

## Topics

### Designating validation data

case split(strategy: MLSplitStrategy)

A validation dataset derived by randomly selecting a portion of the image classifier’s training dataset using the split strategy.

case dataSource(MLImageClassifier.DataSource)

A validation dataset represented by a data source.

case dictionary([String : [URL]])

A validation dataset represented by a dictionary.

Deprecated

case none

An empty validation dataset that skips the model validation phase after training.

## Relationships

### Conforms To

- Sendable

## See Also

### Supporting types

enum FeatureExtractorType

The underlying base model that extracts image features for image classifier training session.

struct ImageAugmentationOptions

The variations that the training process can use to generate more training data from the training data you provide.

