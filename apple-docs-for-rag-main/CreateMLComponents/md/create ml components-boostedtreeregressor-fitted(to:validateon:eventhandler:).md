

- Create ML Components
- BoostedTreeRegressor
-  fitted(to:validateOn:eventHandler:) 

Instance Method

# fitted(to:validateOn:eventHandler:)

Fits a boosted tree regressor model to a collection of examples.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func fitted(
    to input: DataFrame,
    validateOn validation: DataFrame? = nil,
    eventHandler: EventHandler? = nil
) async throws -> TreeRegressorModel
```

## Parameters 

`input`  

A data frame containing examples used for fitting the transformer.

`validation`  

A data frame containing examples used for validating the fitted transformer.

`eventHandler`  

An event handler. This method reports maximum error and root-mean-square error metrics.

## Return Value

The fitted boosted tree regressor model.

## See Also

### Fitting a regressor model

typealias Transformer

The transformer type created by this estimator.

