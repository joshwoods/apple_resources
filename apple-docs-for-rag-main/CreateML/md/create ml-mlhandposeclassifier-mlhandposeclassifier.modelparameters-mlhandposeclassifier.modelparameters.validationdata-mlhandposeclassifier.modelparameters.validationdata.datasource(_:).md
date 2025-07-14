

- Create ML
- MLHandPoseClassifier
- MLHandPoseClassifier.ModelParameters
- MLHandPoseClassifier.ModelParameters.ValidationData
-  MLHandPoseClassifier.ModelParameters.ValidationData.dataSource(\_:) 

Case

# MLHandPoseClassifier.ModelParameters.ValidationData.dataSource(\_:)

Creates a validation dataset from a data source.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
case dataSource(MLHandPoseClassifier.DataSource)
```

## Parameters 

`dataSource`  

An MLHandPoseClassifier.DataSource instance.

## See Also

### Designating validation data

case split(strategy: MLSplitStrategy)

Creates a validation dataset by randomly selecting a portion of the hand pose classifier task’s training dataset with a split strategy.

case none

Creates an empty validation dataset, which tells the task to skip the model validation phase in a training session.

