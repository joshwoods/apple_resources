

- Create ML
- MLActivityClassifier
- MLActivityClassifier.ModelParameters
-  MLActivityClassifier.ModelParameters.Validation 

Enumeration

# MLActivityClassifier.ModelParameters.Validation

The source of a validation dataset for an activity classifier.

macOS 14.0+

``` source
enum Validation
```

## Topics

### Specifying validation data

case split(strategy: MLSplitStrategy)

A validation dataset derived by randomly selecting a portion of the training data.

case dataSource(MLActivityClassifier.DataSource)

A validation dataset represented by a data source.

case none

An empty validation dataset that skips the model validation phase after training.

## See Also

### Creating parameters

init(validation: MLActivityClassifier.ModelParameters.Validation, batchSize: Int?, maximumIterations: Int?, predictionWindowSize: Int?)

Creates a set of activity classifier parameters that includes a validation dataset in a data source.

init(validationData: MLActivityClassifier.DataSource, batchSize: Int?, maximumIterations: Int?, predictionWindowSize: Int?)

Creates a set of activity classifier parameters that includes a validation dataset in a data source.

init(validationData: MLDataTable?, batchSize: Int?, maximumIterations: Int?, predictionWindowSize: Int?)

Creates a set of activity classifier parameters that includes a validation dataset in a data table.

Deprecated

