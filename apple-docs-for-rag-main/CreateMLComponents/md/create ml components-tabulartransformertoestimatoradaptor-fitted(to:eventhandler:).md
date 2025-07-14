

- Create ML Components
- TabularTransformerToEstimatorAdaptor
-  fitted(to:eventHandler:) 

Instance Method

# fitted(to:eventHandler:)

Returns the pre-defined tabular transformer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func fitted(
    to input: DataFrame,
    eventHandler: EventHandler? = nil
) async throws -> Transformer
```

## Parameters 

`input`  

A data frame.

`eventHandler`  

An event handler.

## Return Value

The pre-defined tabular transformer.

