

- Create ML Components
- MultivariateLinearRegressor
- MultivariateLinearRegressor.Model
-  applied(to:eventHandler:) 

Instance Method

# applied(to:eventHandler:)

Performs a prediction on a shaped array.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func applied(
    to input: MLShapedArray,
    eventHandler: EventHandler? = nil
) async throws -> MLShapedArray
```

## Parameters 

`input`  

A shaped array of features. The last dimension must be `inputSize`.

`eventHandler`  

An event handler.

## Return Value

A shaped array of predictions. The shape of the predictions matches the shape of the input except for the last dimension, which is `outputSize`.

