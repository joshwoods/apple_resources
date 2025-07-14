

- Create ML
- MLActivityClassifier
- MLActivityClassifier.ModelParameters
-  predictionWindowSize 

Instance Property

# predictionWindowSize

The number of samples for each labeled activity.

macOS 10.15+

``` source
var predictionWindowSize: Int?
```

## See Also

### Accessing the training parameters

var validationData: MLDataTable?

The activity classifier’s validation dataset.

Deprecated

var batchSize: Int?

The number of sequence chunks the training session uses per iteration.

var maximumIterations: Int?

The maximum number of iterations over the training data the training session uses.

var validation: MLActivityClassifier.ModelParameters.Validation

The validation data source.

