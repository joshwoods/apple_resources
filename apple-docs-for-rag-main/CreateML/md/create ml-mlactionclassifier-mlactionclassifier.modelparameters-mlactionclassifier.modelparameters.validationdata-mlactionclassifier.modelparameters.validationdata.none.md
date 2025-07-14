

- Create ML
- MLActionClassifier
- MLActionClassifier.ModelParameters
- MLActionClassifier.ModelParameters.ValidationData
-  MLActionClassifier.ModelParameters.ValidationData.none 

Case

# MLActionClassifier.ModelParameters.ValidationData.none

An empty validation dataset that skips the model validation phase after training.

macOS 11.0+

``` source
case none
```

## Discussion

Use this case when you don’t have validation data while preventing Create ML from using any of your training dataset for validation.

## See Also

### Designating validation data

case dataSource(MLActionClassifier.DataSource)

A validation dataset represented by a data source.

case split(strategy: MLSplitStrategy)

A validation dataset derived by randomly selecting a portion of the action classifier’s training dataset using the split strategy.

