

- Create ML
- MLActivityClassifier
- MLActivityClassifier.ModelParameters
- MLActivityClassifier.ModelParameters.Validation
-  MLActivityClassifier.ModelParameters.Validation.dataSource(\_:) 

Case

# MLActivityClassifier.ModelParameters.Validation.dataSource(\_:)

A validation dataset represented by a data source.

macOS 14.0+

``` source
case dataSource(MLActivityClassifier.DataSource)
```

## See Also

### Specifying validation data

case split(strategy: MLSplitStrategy)

A validation dataset derived by randomly selecting a portion of the training data.

case none

An empty validation dataset that skips the model validation phase after training.

