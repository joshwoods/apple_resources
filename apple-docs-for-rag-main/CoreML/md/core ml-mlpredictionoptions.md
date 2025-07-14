

- Core ML
-  MLPredictionOptions 

Class

# MLPredictionOptions

The options available when making a prediction.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class MLPredictionOptions
```

## Topics

### Getting features

var outputBackings: [String : Any]

A dictionary of feature names and client-allocated buffers.

### Restricting computation to the CPU

var usesCPUOnly: Bool

A Boolean value that indicates whether a prediction is computed using only the CPU.

Deprecated

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

