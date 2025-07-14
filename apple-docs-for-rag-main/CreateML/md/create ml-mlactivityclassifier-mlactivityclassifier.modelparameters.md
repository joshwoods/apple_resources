

- Create ML
- MLActivityClassifier
-  MLActivityClassifier.ModelParameters 

Structure

# MLActivityClassifier.ModelParameters

Model training parameters that direct the training process for an activity classifier model.

macOS 10.15+

``` source
struct ModelParameters
```

## Topics

### Creating parameters

init(validation: MLActivityClassifier.ModelParameters.Validation, batchSize: Int?, maximumIterations: Int?, predictionWindowSize: Int?)

Creates a set of activity classifier parameters that includes a validation dataset in a data source.

init(validationData: MLActivityClassifier.DataSource, batchSize: Int?, maximumIterations: Int?, predictionWindowSize: Int?)

Creates a set of activity classifier parameters that includes a validation dataset in a data source.

init(validationData: MLDataTable?, batchSize: Int?, maximumIterations: Int?, predictionWindowSize: Int?)

Creates a set of activity classifier parameters that includes a validation dataset in a data table.

Deprecated

enum Validation

The source of a validation dataset for an activity classifier.

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

var validation: MLActivityClassifier.ModelParameters.Validation

The validation data source.

### Describing parameters

var description: String

A text representation of the activity-model parameters.

var debugDescription: String

A text representation of the activity-model parameters that’s suitable for output during debugging.

var playgroundDescription: Any

A description of the activity-model parameters shown in a playground.

### Default Implementations

CustomDebugStringConvertible Implementations

CustomPlaygroundDisplayConvertible Implementations

CustomStringConvertible Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomPlaygroundDisplayConvertible
- CustomStringConvertible

## See Also

### Supporting types

enum DataSource

A data source for an activity classifier.

