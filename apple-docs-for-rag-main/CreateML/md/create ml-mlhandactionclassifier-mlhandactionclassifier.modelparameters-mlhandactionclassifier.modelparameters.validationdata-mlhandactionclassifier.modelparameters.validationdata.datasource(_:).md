

- Create ML
- MLHandActionClassifier
- MLHandActionClassifier.ModelParameters
- MLHandActionClassifier.ModelParameters.ValidationData
-  MLHandActionClassifier.ModelParameters.ValidationData.dataSource(\_:) 

Case

# MLHandActionClassifier.ModelParameters.ValidationData.dataSource(\_:)

Creates a validation dataset from a data source.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
case dataSource(MLHandActionClassifier.DataSource)
```

## Discussion

- dataSource: An MLHandActionClassifier.DataSource instance.

## See Also

### Designating validation data

case split(strategy: MLSplitStrategy)

Creates a validation dataset by randomly selecting a portion of the hand action classifier task’s training dataset with a split strategy.

case none

Creates an empty validation dataset, which tells the task to skip the model validation phase in a training session.

