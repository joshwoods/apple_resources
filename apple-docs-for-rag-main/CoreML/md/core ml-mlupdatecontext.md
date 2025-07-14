

- Core ML
-  MLUpdateContext 

Class

# MLUpdateContext

The context an update task provides to your app’s completion and update progress handlers.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 14.0+visionOS 1.0+watchOS 6.0+

``` source
class MLUpdateContext
```

## Topics

### Getting the Update Context

var event: MLUpdateProgressEvent

The event type that triggered an update task to notify your app’s completion and update progress handlers.

struct MLUpdateProgressEvent

A type of event during a model update task.

var task: MLUpdateTask

The update task that generated the update context.

var parameters: [MLParameterKey : Any]

The parameters for the update task.

class MLParameterKey

The keys for the parameter dictionary in a model configuration or a model update context.

### Evaluating the Update

var metrics: [MLMetricKey : Any]

The training metrics of the model for the update task, contained in a dictionary.

class MLMetricKey

A key for the metrics dictionary in an update context.

### Saving an Updated Model

var model: any MLModel &amp; MLWritable

The underlying Core ML model stored in memory.

protocol MLWritable

A set of methods that saves a machine learning type to the file system.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Creating an Update Task

convenience init(forModelAt: URL, trainingData: any MLBatchProvider, completionHandler: (MLUpdateContext) -> Void) throws

Creates a task that updates the model at the URL with the training data, and calls the completion handler when the update completes.

convenience init(forModelAt: URL, trainingData: any MLBatchProvider, progressHandlers: MLUpdateProgressHandlers) throws

Creates a task that updates the model at the URL with the training data, and calls the progress handlers during and after the update.

convenience init(forModelAt: URL, trainingData: any MLBatchProvider, configuration: MLModelConfiguration?, completionHandler: (MLUpdateContext) -> Void) throws

Creates a task that updates the model at the URL with the training data and configuration, and calls the completion handler when the update completes.

convenience init(forModelAt: URL, trainingData: any MLBatchProvider, configuration: MLModelConfiguration?, progressHandlers: MLUpdateProgressHandlers) throws

Creates a task that updates the model at the URL with the training data and configuration, and calls the progress handlers during and after the update.

convenience init(forModelAtURL: URL, trainingData: any MLBatchProvider, completionHandler: (MLUpdateContext) -> Void) throws

convenience init(forModelAtURL: URL, trainingData: any MLBatchProvider, progressHandlers: MLUpdateProgressHandlers) throws

convenience init(forModelAtURL: URL, trainingData: any MLBatchProvider, configuration: MLModelConfiguration?, completionHandler: (MLUpdateContext) -> Void) throws

convenience init(forModelAtURL: URL, trainingData: any MLBatchProvider, configuration: MLModelConfiguration?, progressHandlers: MLUpdateProgressHandlers) throws

protocol MLBatchProvider

An interface that represents a collection of feature providers.

class MLModelConfiguration

The settings for creating or updating a machine learning model.

class MLUpdateProgressHandlers

A collection of closures an update task uses to notify your app of its progress.

