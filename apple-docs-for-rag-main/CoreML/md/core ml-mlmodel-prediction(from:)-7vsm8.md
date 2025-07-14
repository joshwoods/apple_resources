

- Core ML
- MLModel
-  prediction(from:) 

Instance Method

# prediction(from:)

Run a prediction on a model.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func prediction(from inputs: [String : MLTensor]) async throws -> [String : MLTensor]
```

## Parameters 

`inputs`  

The named input, or inputs, to make a prediction from.

## Return Value

The output, or outputs, from the prediction.

## Discussion

This method requires all inputs and outputs to be multidimensional arrays. If your model doesn’t satisfy this requirement, materialize the tensor inputs to `MLShapedArray` values to create feature values for each, for example:

```
let shapedArray = await tensor.shapedArray(of: Float.self)
let inputFeatures = try MLDictionaryFeatureProvider(dictionary: [
    "x": MLFeatureValue(shapedArray: shapedArray),
    // Other non-multidimensional array inputs
])
let prediction = try await model.prediction(from: inputFeatures)
```

## See Also

### Making Predictions

func prediction(from: any MLFeatureProvider) throws -> any MLFeatureProvider

Generates a prediction from the feature values within the input feature provider.

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

