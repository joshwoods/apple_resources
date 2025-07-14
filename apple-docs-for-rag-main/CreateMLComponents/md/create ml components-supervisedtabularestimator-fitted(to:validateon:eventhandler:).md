

- Create ML Components
- SupervisedTabularEstimator
-  fitted(to:validateOn:eventHandler:) 

Instance Method

# fitted(to:validateOn:eventHandler:)

Fits a transformer to a data frame

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func fitted(
    to input: DataFrame,
    validateOn validation: DataFrame?,
    eventHandler: EventHandler?
) async throws -> Self.Transformer
```

**Required**

## Parameters 

`input`  

A data frame containing examples used for fitting the transformer.

`validation`  

A data frame containing examples used for validating the fitted transformer.

`eventHandler`  

An event handler.

## Return Value

The fitted transformer.

## See Also

### Fitting

func fitted(to: DataFrame, validateOn: DataFrame?) async throws -> Self.Transformer

