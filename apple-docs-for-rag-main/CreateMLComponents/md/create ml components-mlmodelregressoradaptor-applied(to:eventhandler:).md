

- Create ML Components
- MLModelRegressorAdaptor
-  applied(to:eventHandler:) 

Instance Method

# applied(to:eventHandler:)

Performs a prediction from a single input.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func applied(
    to input: MLShapedArray,
    eventHandler: EventHandler? = nil
) async throws -> Double
```

## Parameters 

`input`  

The input feature.

`eventHandler`  

An event handler.

## Return Value

A regression result.

