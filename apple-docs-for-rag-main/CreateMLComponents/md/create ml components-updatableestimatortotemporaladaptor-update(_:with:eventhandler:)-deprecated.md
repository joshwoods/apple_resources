

- Create ML Components
- UpdatableEstimatorToTemporalAdaptor
-  update(\_:with:eventHandler:) Deprecated

Instance Method

# update(\_:with:eventHandler:)

Updates a transformer with a new sequence of examples.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func update(
    _ transformer: inout UpdatableEstimatorToTemporalAdaptor.Transformer,
    with input: InputSequence,
    eventHandler: EventHandler? = nil
) async throws where InputSequence : Sequence, InputSequence.Element : TemporalSequence, Base.Transformer.Input == InputSequence.Element.Feature
```

## Parameters 

`transformer`  

A transformer to update.

`input`  

A sequence of examples.

`eventHandler`  

An event handler.

## See Also

### Fitting and updating

func fitted&lt;InputSequence>(to: InputSequence, eventHandler: EventHandler?) async throws -> UpdatableEstimatorToTemporalAdaptor&lt;Base>.Transformer

Fits a transformer to a sequence of examples.

Deprecated

func makeTransformer() -> UpdatableEstimatorToTemporalAdaptor&lt;Base>.Transformer

Creates a default-initialized transformer suitable for incremental fitting.

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

