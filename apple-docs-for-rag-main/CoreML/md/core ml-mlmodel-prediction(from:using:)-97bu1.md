

- Core ML
- MLModel
-  prediction(from:using:) 

Instance Method

# prediction(from:using:)

Run a stateful prediction synchronously.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func prediction(
    from inputFeatures: any MLFeatureProvider,
    using state: MLState
) throws -> any MLFeatureProvider
```

## Discussion

Use this method to run predictions on a stateful model.

```
let state = model.newState()
let prediction = try model.prediction(from: inputFeatures, using: state)
```

- inputFeatures: The input features as declared in the model description.

- state: The state object created by `newState()` method.

- error: The output parameter to receive an error information on failure.

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

func prediction(from: any MLFeatureProvider, using: MLState, options: MLPredictionOptions) async throws -> any MLFeatureProvider

Run a stateful prediction on a model asynchronously.

func prediction(from: any MLFeatureProvider, using: MLState, options: MLPredictionOptions) throws -> any MLFeatureProvider

Run a stateful prediction synchronously with options.

class MLPredictionOptions

The options available when making a prediction.

