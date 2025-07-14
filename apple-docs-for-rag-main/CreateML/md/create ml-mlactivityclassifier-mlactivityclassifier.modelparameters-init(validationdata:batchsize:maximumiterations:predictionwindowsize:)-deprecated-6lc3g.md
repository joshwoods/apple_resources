

- Create ML
- MLActivityClassifier
- MLActivityClassifier.ModelParameters
-  init(validationData:batchSize:maximumIterations:predictionWindowSize:) Deprecated

Initializer

# init(validationData:batchSize:maximumIterations:predictionWindowSize:)

Creates a set of activity classifier parameters that includes a validation dataset in a data table.

macOS 10.15–14.0Deprecated

``` source
init(
    validationData: MLDataTable?,
    batchSize: Int? = 32,
    maximumIterations: Int? = 10,
    predictionWindowSize: Int? = 100
)
```

## Parameters 

`validationData`  

An MLDataTable instance that contains a validation dataset.

`batchSize`  

The number of activity entries the training session uses for each of its training iterations.

`maximumIterations`  

The largest number of training iterations the training session can use.

`predictionWindowSize`  

The number of time increments the training session uses to train an activity classifier.

## See Also

### Creating parameters

init(validation: MLActivityClassifier.ModelParameters.Validation, batchSize: Int?, maximumIterations: Int?, predictionWindowSize: Int?)

Creates a set of activity classifier parameters that includes a validation dataset in a data source.

init(validationData: MLActivityClassifier.DataSource, batchSize: Int?, maximumIterations: Int?, predictionWindowSize: Int?)

Creates a set of activity classifier parameters that includes a validation dataset in a data source.

enum Validation

The source of a validation dataset for an activity classifier.

