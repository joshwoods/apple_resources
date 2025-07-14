

- Create ML
- MLActionClassifier
- MLActionClassifier.ModelParameters
- MLActionClassifier.ModelParameters.ValidationData
-  MLActionClassifier.ModelParameters.ValidationData.dataSource(\_:) 

Case

# MLActionClassifier.ModelParameters.ValidationData.dataSource(\_:)

A validation dataset represented by a data source.

macOS 11.0+

``` source
case dataSource(MLActionClassifier.DataSource)
```

## See Also

### Designating validation data

case split(strategy: MLSplitStrategy)

A validation dataset derived by randomly selecting a portion of the action classifier’s training dataset using the split strategy.

case none

An empty validation dataset that skips the model validation phase after training.

