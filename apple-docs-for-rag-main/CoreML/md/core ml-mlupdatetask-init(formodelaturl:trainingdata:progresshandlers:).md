

- Core ML
- MLUpdateTask
-  init(forModelAtURL:trainingData:progressHandlers:) 

Initializer

# init(forModelAtURL:trainingData:progressHandlers:)

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
convenience init(
    forModelAtURL modelURL: URL,
    trainingData: any MLBatchProvider,
    progressHandlers: MLUpdateProgressHandlers
) throws
```

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

convenience init(forModelAtURL: URL, trainingData: any MLBatchProvider, configuration: MLModelConfiguration?, completionHandler: (MLUpdateContext) -> Void) throws

convenience init(forModelAtURL: URL, trainingData: any MLBatchProvider, configuration: MLModelConfiguration?, progressHandlers: MLUpdateProgressHandlers) throws

protocol MLBatchProvider

An interface that represents a collection of feature providers.

class MLModelConfiguration

The settings for creating or updating a machine learning model.

class MLUpdateContext

The context an update task provides to your app’s completion and update progress handlers.

class MLUpdateProgressHandlers

A collection of closures an update task uses to notify your app of its progress.

