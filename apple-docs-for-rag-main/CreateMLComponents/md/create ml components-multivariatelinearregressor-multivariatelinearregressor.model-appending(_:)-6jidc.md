

- Create ML Components
- MultivariateLinearRegressor
- MultivariateLinearRegressor.Model
-  appending(\_:) 

Instance Method

# appending(\_:)

Composes this transformer with a prediction-only transformer.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
func appending(_ other: Other) -> some Transformer> where Other : Transformer, Self.Output == AnnotatedPrediction
```

