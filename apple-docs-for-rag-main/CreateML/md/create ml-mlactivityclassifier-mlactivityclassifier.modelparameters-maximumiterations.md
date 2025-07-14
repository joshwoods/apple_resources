

- Create ML
- MLActivityClassifier
- MLActivityClassifier.ModelParameters
-  maximumIterations 

Instance Property

# maximumIterations

The maximum number of iterations over the training data the training session uses.

macOS 10.15+

``` source
var maximumIterations: Int?
```

## See Also

### Accessing the training parameters

var validationData: MLDataTable?

The activity classifier’s validation dataset.

Deprecated

var batchSize: Int?

The number of sequence chunks the training session uses per iteration.

var predictionWindowSize: Int?

The number of samples for each labeled activity.

var validation: MLActivityClassifier.ModelParameters.Validation

The validation data source.

