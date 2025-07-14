

- Core ML
- MLModel
-  predictions(fromBatch:) 

Instance Method

# predictions(fromBatch:)

Generates predictions for each input feature provider within the batch provider.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
func predictions(fromBatch inputBatch: any MLBatchProvider) throws -> any MLBatchProvider
```

## Parameters 

`inputBatch`  

A batch provider that contains multiple input feature providers. The model makes a prediction for each feature provider.

## Return Value

A batch provider that contains an output feature provider for each prediction.

## Discussion

Use this method to make more than one prediction at one time.

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

