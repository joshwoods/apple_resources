

- Create ML Components
- ColumnSelectorTransformer
-  applied(to:eventHandler:) 

Instance Method

# applied(to:eventHandler:)

Performs the transformation on selected columns of the data frame.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func applied(
    to input: DataFrame,
    eventHandler: EventHandler? = nil
) async throws -> DataFrame
```

## Parameters 

`input`  

A data frame.

`eventHandler`  

An event handler.

## Return Value

A data frame produced by applying the transformer to selected columns.

