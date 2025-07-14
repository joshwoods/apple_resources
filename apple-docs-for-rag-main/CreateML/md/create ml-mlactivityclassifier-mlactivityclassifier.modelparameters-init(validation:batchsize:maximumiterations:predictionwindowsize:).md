

- Create ML
- MLActivityClassifier
- MLActivityClassifier.ModelParameters
-  init(validation:batchSize:maximumIterations:predictionWindowSize:) 

Initializer

# init(validation:batchSize:maximumIterations:predictionWindowSize:)

Creates a set of activity classifier parameters that includes a validation dataset in a data source.

macOS 14.0+

``` source
init(
    validation: MLActivityClassifier.ModelParameters.Validation = .split(strategy: .automatic),
    batchSize: Int? = 32,
    maximumIterations: Int? = 10,
    predictionWindowSize: Int? = 100
)
```

## Parameters 

`validation`  

An MLActivityClassifier.DataSource instance that contains a validation dataset.

`batchSize`  

The number of activity entries the training session uses for each of its training iterations.

`maximumIterations`  

The largest number of training iterations the training session can use.

`predictionWindowSize`  

The number of time increments the training session uses to train an activity classifier.

## See Also

### Creating parameters

init(validationData: MLActivityClassifier.DataSource, batchSize: Int?, maximumIterations: Int?, predictionWindowSize: Int?)

Creates a set of activity classifier parameters that includes a validation dataset in a data source.

init(validationData: MLDataTable?, batchSize: Int?, maximumIterations: Int?, predictionWindowSize: Int?)

Creates a set of activity classifier parameters that includes a validation dataset in a data table.

Deprecated

enum Validation

The source of a validation dataset for an activity classifier.

