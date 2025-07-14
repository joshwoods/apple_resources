

- Create ML Components
- UpdatableTabularEstimatorToSupervisedAdaptor
-  fitted(to:validateOn:eventHandler:) 

Instance Method

# fitted(to:validateOn:eventHandler:)

Fits a transformer to a data frame.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func fitted(
    to input: DataFrame,
    validateOn validation: DataFrame?,
    eventHandler: EventHandler? = nil
) async throws -> UpdatableTabularEstimatorToSupervisedAdaptor.Transformer
```

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

func makeTransformer() -> Estimator.Transformer

Creates a default-initialized transformer suitable for incremental fitting.

func update(inout UpdatableTabularEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer, with: DataFrame, eventHandler: EventHandler?) async throws

Updates a transformer with a new data frame containing examples.

typealias Transformer

The transformer type created by this estimator.

