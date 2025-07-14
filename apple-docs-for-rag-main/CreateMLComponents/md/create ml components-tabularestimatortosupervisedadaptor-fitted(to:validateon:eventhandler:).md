

- Create ML Components
- TabularEstimatorToSupervisedAdaptor
-  fitted(to:validateOn:eventHandler:) 

Instance Method

# fitted(to:validateOn:eventHandler:)

Returns the tabular transformer fitted using the provided tabular estimator.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func fitted(
    to input: DataFrame,
    validateOn validation: DataFrame? = nil,
    eventHandler: EventHandler? = nil
) async throws -> Estimator.Transformer
```

## Parameters 

`input`  

A data frame containing examples.

`validation`  

A data frame containing examples.

`eventHandler`  

An event handler.

## Return Value

The a fitted tabular transformer.

## See Also

### Fitting

typealias Transformer

The transformer type created by this estimator.

