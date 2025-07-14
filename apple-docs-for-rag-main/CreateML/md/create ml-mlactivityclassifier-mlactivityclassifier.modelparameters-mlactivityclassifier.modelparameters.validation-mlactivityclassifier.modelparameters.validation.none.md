

- Create ML
- MLActivityClassifier
- MLActivityClassifier.ModelParameters
- MLActivityClassifier.ModelParameters.Validation
-  MLActivityClassifier.ModelParameters.Validation.none 

Case

# MLActivityClassifier.ModelParameters.Validation.none

An empty validation dataset that skips the model validation phase after training.

macOS 14.0+

``` source
case none
```

## See Also

### Specifying validation data

case split(strategy: MLSplitStrategy)

A validation dataset derived by randomly selecting a portion of the training data.

case dataSource(MLActivityClassifier.DataSource)

A validation dataset represented by a data source.

