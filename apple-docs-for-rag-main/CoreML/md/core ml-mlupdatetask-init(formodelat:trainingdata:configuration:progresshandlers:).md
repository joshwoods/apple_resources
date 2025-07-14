

- Core ML
- MLUpdateTask
-  init(forModelAt:trainingData:configuration:progressHandlers:) 

Initializer

# init(forModelAt:trainingData:configuration:progressHandlers:)

Creates a task that updates the model at the URL with the training data and configuration, and calls the progress handlers during and after the update.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 14.0+visionOS 1.0+watchOS 6.0+

``` source
convenience init(
    forModelAt modelURL: URL,
    trainingData: any MLBatchProvider,
    configuration: MLModelConfiguration?,
    progressHandlers: MLUpdateProgressHandlers
) throws
```

## Parameters 

`modelURL`  

The location in the file system of a model file (*ModelName*`.mlmodelc`).

`trainingData`  

The update data for the model, contained in a batch provider.

`configuration`  

The model settings for an updated model object.

`progressHandlers`  

The closures the task calls during the update process.

## See Also

### Creating an Update Task

convenience init(forModelAt: URL, trainingData: any MLBatchProvider, completionHandler: (MLUpdateContext) -> Void) throws

Creates a task that updates the model at the URL with the training data, and calls the completion handler when the update completes.

convenience init(forModelAt: URL, trainingData: any MLBatchProvider, progressHandlers: MLUpdateProgressHandlers) throws

Creates a task that updates the model at the URL with the training data, and calls the progress handlers during and after the update.

convenience init(forModelAt: URL, trainingData: any MLBatchProvider, configuration: MLModelConfiguration?, completionHandler: (MLUpdateContext) -> Void) throws

Creates a task that updates the model at the URL with the training data and configuration, and calls the completion handler when the update completes.

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

class MLUpdateProgressHandlers

A collection of closures an update task uses to notify your app of its progress.

