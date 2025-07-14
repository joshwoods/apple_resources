

- Create ML Components
- UpdatableTabularEstimatorToSupervisedAdaptor
-  update(\_:with:eventHandler:) 

Instance Method

# update(\_:with:eventHandler:)

Updates a transformer with a new data frame containing examples.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func update(
    _ transformer: inout UpdatableTabularEstimatorToSupervisedAdaptor.Transformer,
    with input: DataFrame,
    eventHandler: EventHandler? = nil
) async throws
```

## Parameters 

`transformer`  

A transformer to update.

`input`  

A sequence of examples.

`eventHandler`  

An event handler.

## See Also

### Fitting

func fitted(to: DataFrame, validateOn: DataFrame?, eventHandler: EventHandler?) async throws -> UpdatableTabularEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer

Fits a transformer to a data frame.

func makeTransformer() -> Estimator.Transformer

Creates a default-initialized transformer suitable for incremental fitting.

typealias Transformer

The transformer type created by this estimator.

