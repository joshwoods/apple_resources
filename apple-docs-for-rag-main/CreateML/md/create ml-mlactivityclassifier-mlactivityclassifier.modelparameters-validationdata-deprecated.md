

- Create ML
- MLActivityClassifier
- MLActivityClassifier.ModelParameters
-  validationData Deprecated

Instance Property

# validationData

The activity classifier’s validation dataset.

macOS 10.15–14.0Deprecated

``` source
var validationData: MLDataTable?
```

Deprecated

Use validationDataSource

## Discussion

If you don’t specify validation data, the training process automatically sets aside a random subset of the training data as the validation data.

## See Also

### Accessing the training parameters

var batchSize: Int?

The number of sequence chunks the training session uses per iteration.

var maximumIterations: Int?

The maximum number of iterations over the training data the training session uses.

var predictionWindowSize: Int?

The number of samples for each labeled activity.

var validation: MLActivityClassifier.ModelParameters.Validation

The validation data source.

