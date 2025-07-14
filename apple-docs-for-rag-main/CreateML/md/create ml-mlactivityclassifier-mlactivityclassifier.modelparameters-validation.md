

- Create ML
- MLActivityClassifier
- MLActivityClassifier.ModelParameters
-  validation 

Instance Property

# validation

The validation data source.

macOS 14.0+

``` source
var validation: MLActivityClassifier.ModelParameters.Validation { get set }
```

## Discussion

If you don’t specify validation data, the training process automatically sets aside a random subset of the training data as the validation data.

## See Also

### Accessing the training parameters

var validationData: MLDataTable?

The activity classifier’s validation dataset.

Deprecated

var batchSize: Int?

The number of sequence chunks the training session uses per iteration.

var maximumIterations: Int?

The maximum number of iterations over the training data the training session uses.

var predictionWindowSize: Int?

The number of samples for each labeled activity.

