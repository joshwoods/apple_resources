

- Create ML
- MLActivityClassifier
- MLActivityClassifier.ModelParameters
-  batchSize 

Instance Property

# batchSize

The number of sequence chunks the training session uses per iteration.

macOS 10.15+

``` source
var batchSize: Int?
```

## See Also

### Accessing the training parameters

var validationData: MLDataTable?

The activity classifier’s validation dataset.

Deprecated

var maximumIterations: Int?

The maximum number of iterations over the training data the training session uses.

var predictionWindowSize: Int?

The number of samples for each labeled activity.

var validation: MLActivityClassifier.ModelParameters.Validation

The validation data source.

