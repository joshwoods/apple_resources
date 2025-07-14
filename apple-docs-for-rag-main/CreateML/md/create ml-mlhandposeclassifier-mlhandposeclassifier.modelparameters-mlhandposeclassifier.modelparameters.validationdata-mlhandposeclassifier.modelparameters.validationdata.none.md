

- Create ML
- MLHandPoseClassifier
- MLHandPoseClassifier.ModelParameters
- MLHandPoseClassifier.ModelParameters.ValidationData
-  MLHandPoseClassifier.ModelParameters.ValidationData.none 

Case

# MLHandPoseClassifier.ModelParameters.ValidationData.none

Creates an empty validation dataset, which tells the task to skip the model validation phase in a training session.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
case none
```

## Discussion

This case prevents Create ML from creating a validation dataset from your training dataset. You typically use it when your training dataset is small and can’t spare any data to validate the model.

## See Also

### Designating validation data

case dataSource(MLHandPoseClassifier.DataSource)

Creates a validation dataset from a data source.

case split(strategy: MLSplitStrategy)

Creates a validation dataset by randomly selecting a portion of the hand pose classifier task’s training dataset with a split strategy.

