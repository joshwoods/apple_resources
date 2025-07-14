

- Create ML
- MLActionClassifier
- MLActionClassifier.ModelParameters
- MLActionClassifier.ModelParameters.ValidationData
-  MLActionClassifier.ModelParameters.ValidationData.split(strategy:) 

Case

# MLActionClassifier.ModelParameters.ValidationData.split(strategy:)

A validation dataset derived by randomly selecting a portion of the action classifier’s training dataset using the split strategy.

macOS 11.0+

``` source
case split(strategy: MLSplitStrategy)
```

## See Also

### Designating validation data

case dataSource(MLActionClassifier.DataSource)

A validation dataset represented by a data source.

case none

An empty validation dataset that skips the model validation phase after training.

