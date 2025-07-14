

- Create ML
- MLHandActionClassifier
- MLHandActionClassifier.ModelParameters
-  MLHandActionClassifier.ModelParameters.ValidationData 

Enumeration

# MLHandActionClassifier.ModelParameters.ValidationData

A dataset a hand action classifier task uses to validate the model during a training session.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
enum ValidationData
```

## Topics

### Designating validation data

case dataSource(MLHandActionClassifier.DataSource)

Creates a validation dataset from a data source.

case split(strategy: MLSplitStrategy)

Creates a validation dataset by randomly selecting a portion of the hand action classifier task’s training dataset with a split strategy.

case none

Creates an empty validation dataset, which tells the task to skip the model validation phase in a training session.

## See Also

### Parameter supporting types

struct VideoAugmentationOptions

Options a hand action classification training session can use to generate additional training data from the videos you provide.

enum ModelAlgorithmType

The hand action classifier training algorithm options.

