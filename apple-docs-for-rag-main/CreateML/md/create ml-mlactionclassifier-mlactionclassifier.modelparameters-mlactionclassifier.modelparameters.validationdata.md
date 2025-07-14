

- Create ML
- MLActionClassifier
- MLActionClassifier.ModelParameters
-  MLActionClassifier.ModelParameters.ValidationData 

Enumeration

# MLActionClassifier.ModelParameters.ValidationData

The source of a validation dataset for an action classifier.

macOS 11.0+

``` source
enum ValidationData
```

## Topics

### Designating validation data

case dataSource(MLActionClassifier.DataSource)

A validation dataset represented by a data source.

case split(strategy: MLSplitStrategy)

A validation dataset derived by randomly selecting a portion of the action classifier’s training dataset using the split strategy.

case none

An empty validation dataset that skips the model validation phase after training.

## See Also

### Supporting types

struct VideoAugmentationOptions

The video augmentations for an action classifier training session.

enum ModelAlgorithmType

The action classifier training algorithm options.

