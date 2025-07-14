

- Core ML
- MLCustomModel
-  predictions(from:options:) 

Instance Method

# predictions(from:options:)

Predicts output values from the given batch of input features.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
optional func predictions(
    from inputBatch: any MLBatchProvider,
    options: MLPredictionOptions
) throws -> any MLBatchProvider
```

## Parameters 

`inputBatch`  

The batch of feature values the model needs to make its predictions.

`options`  

The options to be applied to the predictions.

## Return Value

A batch provider that represents the model’s predictions for the batch of inputs.

## See Also

### Making Predictions

func prediction(from: any MLFeatureProvider, options: MLPredictionOptions) throws -> any MLFeatureProvider

Predicts output values from the given input features.

**Required**

