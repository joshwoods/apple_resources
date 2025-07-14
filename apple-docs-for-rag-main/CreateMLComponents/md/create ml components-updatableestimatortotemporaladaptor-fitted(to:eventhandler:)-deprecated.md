

- Create ML Components
- UpdatableEstimatorToTemporalAdaptor
-  fitted(to:eventHandler:) Deprecated

Instance Method

# fitted(to:eventHandler:)

Fits a transformer to a sequence of examples.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func fitted(
    to input: InputSequence,
    eventHandler: EventHandler? = nil
) async throws -> UpdatableEstimatorToTemporalAdaptor.Transformer where InputSequence : Sequence, InputSequence.Element : TemporalSequence, Base.Transformer.Input == InputSequence.Element.Feature
```

## Parameters 

`input`  

A sequence of examples.

`eventHandler`  

An event handler.

## Return Value

The fitted transformer.

## See Also

### Fitting and updating

func makeTransformer() -> UpdatableEstimatorToTemporalAdaptor&lt;Base>.Transformer

Creates a default-initialized transformer suitable for incremental fitting.

Deprecated

func update&lt;InputSequence>(inout UpdatableEstimatorToTemporalAdaptor&lt;Base>.Transformer, with: InputSequence, eventHandler: EventHandler?) async throws

Updates a transformer with a new sequence of examples.

Deprecated

typealias Input

The input type.

Deprecated

typealias Output

The output type.

Deprecated

typealias Transformer

The transformer type created by this estimator.

Deprecated

