

- Core ML
-  MLUpdateProgressHandlers 

Class

# MLUpdateProgressHandlers

A collection of closures an update task uses to notify your app of its progress.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 14.0+visionOS 1.0+watchOS 6.0+

``` source
class MLUpdateProgressHandlers
```

## Topics

### Creating Progress Handlers

init(forEvents: MLUpdateProgressEvent, progressHandler: ((MLUpdateContext) -> Void)?, completionHandler: (MLUpdateContext) -> Void)

Creates the collection of closures an update task uses to notify your app of its progress.

struct MLUpdateProgressEvent

A type of event during a model update task.

class MLUpdateContext

The context an update task provides to your app’s completion and update progress handlers.

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

class MLUpdateContext

The context an update task provides to your app’s completion and update progress handlers.

