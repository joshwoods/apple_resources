

- Create ML Components
- TreeRegressorModel
-  applied(to:eventHandler:) 

Instance Method

# applied(to:eventHandler:)

Performs a regression on a data frame.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func applied(
    to input: DataFrame,
    eventHandler: EventHandler? = nil
) async throws -> DataFrame
```

## Parameters 

`input`  

The regressor input.

`eventHandler`  

An event handler.

## Return Value

A data frame of regressions.

