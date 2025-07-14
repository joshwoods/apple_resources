

- Create ML
- MLHandPoseClassifier
- MLHandPoseClassifier.ModelParameters
-  MLHandPoseClassifier.ModelParameters.ValidationData 

Enumeration

# MLHandPoseClassifier.ModelParameters.ValidationData

A dataset a hand pose classifier task uses to validate the model during a training session.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
enum ValidationData
```

## Topics

### Designating validation data

case dataSource(MLHandPoseClassifier.DataSource)

Creates a validation dataset from a data source.

case split(strategy: MLSplitStrategy)

Creates a validation dataset by randomly selecting a portion of the hand pose classifier task’s training dataset with a split strategy.

case none

Creates an empty validation dataset, which tells the task to skip the model validation phase in a training session.

## See Also

### Parameter supporting types

struct ImageAugmentationOptions

Options a hand pose classification training session can use to generate additional training data from the images you provide.

enum ModelAlgorithmType

The hand pose classifier training algorithm options.

