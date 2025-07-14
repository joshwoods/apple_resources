

- Core ML
- MLModel
-  prediction(from:) 

Instance Method

# prediction(from:)

Generates a prediction from the feature values within the input feature provider.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func prediction(from input: any MLFeatureProvider) throws -> any MLFeatureProvider
```

## Parameters 

`input`  

A feature provider that stores all the input feature values the model needs for a prediction.

## Return Value

A feature provider that contains the outputs of the prediction.

## Mentioned in 

Creating and Integrating a Model with Custom Layers

## Discussion

Use this method to make a single prediction.

## See Also

### Related Documentation

Making Predictions with a Sequence of Inputs

Integrate a recurrent neural network model to process sequences of inputs.

### Making Predictions

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

