

- Core ML
-  MLModel 

Class

# MLModel

An encapsulation of all the details of your machine learning model.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class MLModel
```

## Mentioned in 

Downloading and Compiling a Model on the User’s Device

Encrypting a Model in Your App

## Overview

MLModel encapsulates a model’s prediction methods, configuration, and model description.

In most cases, you can use Core ML without accessing the MLModel class directly. Instead, use the programmer-friendly wrapper class that Xcode automatically generates when you add a model (see Integrating a Core ML Model into Your App). If your app needs the MLModel interface, use the wrapper class’s `model` property.

With the MLModel interface, you can:

- Make a prediction with your app’s custom MLFeatureProvider by calling prediction(from:) or prediction(from:options:).

- Make multiple predictions with your app’s custom MLBatchProvider by calling predictions(fromBatch:) or predictions(from:options:).

- Inspect your model’s metadata and MLFeatureDescription instances through modelDescription.

If your app downloads and compiles a model on the user’s device, you must use the MLModel class directly to make predictions. See Downloading and Compiling a Model on the User’s Device.

Important

Use an MLModel instance on one thread or one dispatch queue at a time. Do this by either serializing method calls to the model, or by creating a separate model instance for each thread and dispatch queue.

## Topics

### Loading a Model

class func load(contentsOf: URL, configuration: MLModelConfiguration) async throws -> MLModel

Construct a model asynchronously from a compiled model asset.

class func load(MLModelAsset, configuration: MLModelConfiguration, completionHandler: (MLModel?, (any Error)?) -> Void)

Construct a model asynchronously from a compiled model asset.

class func load(contentsOf: URL, configuration: MLModelConfiguration, completionHandler: (Result&lt;MLModel, any Error>) -> Void)

Creates a Core ML model instance asynchronously from a compiled model file, a custom configuration, and a completion handler.

convenience init(contentsOf: URL) throws

Creates a Core ML model instance from a compiled model file.

convenience init(contentsOf: URL, configuration: MLModelConfiguration) throws

Creates a Core ML model instance from a compiled model file and a custom configuration.

convenience init(contentsOfURL: URL) throws

convenience init(contentsOfURL: URL, configuration: MLModelConfiguration) throws

### Compiling a Model

class func compileModel(at: URL) async throws -> URL

Compile a model for a device.

class func compileModel(at: URL, completionHandler: (Result&lt;URL, any Error>) -> Void)

Compile a model for a device.

class func compileModel(at: URL) async throws -> URL

Compile a model for a device.

class func compileModel(at: URL) throws -> URL

Compiles a model on the device to update the model in your app.

Deprecated

### Making Predictions

func prediction(from: any MLFeatureProvider) throws -> any MLFeatureProvider

Generates a prediction from the feature values within the input feature provider.

func prediction(from: [String : MLTensor]) async throws -> [String : MLTensor]

Run a prediction on a model.

func prediction(from: any MLFeatureProvider, options: MLPredictionOptions) throws -> any MLFeatureProvider

Generates a prediction from the feature values within the input feature provider using the prediction options.

func prediction(from: any MLFeatureProvider, options: MLPredictionOptions) async throws -> any MLFeatureProvider

Generates a prediction asynchronously from the feature values within the input feature provider using the prediction options.

func predictions(fromBatch: any MLBatchProvider) throws -> any MLBatchProvider

Generates predictions for each input feature provider within the batch provider.

func predictions(from: any MLBatchProvider, options: MLPredictionOptions) throws -> any MLBatchProvider

Generates a prediction for each input feature provider within the batch provider using the prediction options.

func prediction(from: [String : MLTensor], using: MLState) async throws -> [String : MLTensor]

Run a stateful prediction on a model.

func prediction(from: any MLFeatureProvider, using: MLState) throws -> any MLFeatureProvider

Run a stateful prediction synchronously.

func prediction(from: any MLFeatureProvider, using: MLState, options: MLPredictionOptions) async throws -> any MLFeatureProvider

Run a stateful prediction on a model asynchronously.

func prediction(from: any MLFeatureProvider, using: MLState, options: MLPredictionOptions) throws -> any MLFeatureProvider

Run a stateful prediction synchronously with options.

class MLPredictionOptions

The options available when making a prediction.

### Inspecting a Model

static var availableComputeDevices: [MLComputeDevice]

The list of available compute devices that the model’s prediction methods use.

var configuration: MLModelConfiguration

The configuration of the model set during initialization.

var modelDescription: MLModelDescription

Model information you use at runtime during development, which Xcode also displays in its Core ML model editor view.

class MLModelDescription

Information about a model, primarily the input and output format for each feature the model expects, and optional metadata.

func parameterValue(for: MLParameterKey) throws -> Any

Returns a model parameter value for a key.

class MLParameterKey

The keys for the parameter dictionary in a model configuration or a model update context.

### Supporting Types

class MLModelConfiguration

The settings for creating or updating a machine learning model.

struct MLOptimizationHints

class MLKey

An abstract base class for machine learning key types.

### Instance Methods

func makeState() -> MLState

Creates a new state object.

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

### Core ML models

Getting a Core ML Model

Obtain a Core ML model to use in your app.

Updating a Model File to a Model Package

Convert a Core ML model file into a model package in Xcode.

Integrating a Core ML Model into Your App

Add a simple model to an app, pass input data to the model, and process the model’s predictions.

Model Customization

Expand and modify your model with new layers.

Model Personalization

Update your model to adapt to new data.

