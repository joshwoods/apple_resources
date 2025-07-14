

- Create ML
- MLActivityClassifier
- MLActivityClassifier.ModelParameters
- MLActivityClassifier.ModelParameters.Validation
-  MLActivityClassifier.ModelParameters.Validation.split(strategy:) 

Case

# MLActivityClassifier.ModelParameters.Validation.split(strategy:)

A validation dataset derived by randomly selecting a portion of the training data.

macOS 14.0+

``` source
case split(strategy: MLSplitStrategy)
```

## See Also

### Specifying validation data

case dataSource(MLActivityClassifier.DataSource)

A validation dataset represented by a data source.

case none

An empty validation dataset that skips the model validation phase after training.

