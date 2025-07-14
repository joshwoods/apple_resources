

- Core ML
- MLCustomModel
-  prediction(from:options:) 

Instance Method

# prediction(from:options:)

Predicts output values from the given input features.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
func prediction(
    from input: any MLFeatureProvider,
    options: MLPredictionOptions
) throws -> any MLFeatureProvider
```

**Required**

## Parameters 

`input`  

The feature values the models needs to make its prediction.

`options`  

The options to be applied to the prediction.

## Return Value

A feature provider that represents the model’s prediction.

## See Also

### Making Predictions

func predictions(from: any MLBatchProvider, options: MLPredictionOptions) throws -> any MLBatchProvider

Predicts output values from the given batch of input features.

