

- Create ML Components
- ColumnSelector
-  fitted(to:eventHandler:) 

Instance Method

# fitted(to:eventHandler:)

Fits a transformer to a data frame

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func fitted(
    to input: DataFrame,
    eventHandler: EventHandler? = nil
) async throws -> ColumnSelector.Transformer
```

## Parameters 

`input`  

A data frame.

`eventHandler`  

An event handler.

## Return Value

The fitted transformer.

## See Also

### Fitting a transformer

typealias Input

typealias Output

typealias Transformer

The transformer type created by this estimator.

