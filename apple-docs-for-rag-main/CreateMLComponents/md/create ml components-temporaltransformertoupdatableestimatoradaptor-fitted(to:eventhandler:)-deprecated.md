

- Create ML Components
- TemporalTransformerToUpdatableEstimatorAdaptor
-  fitted(to:eventHandler:) Deprecated

Instance Method

# fitted(to:eventHandler:)

Returns the pre-defined transformer.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func fitted(
    to input: InputSequence,
    eventHandler: EventHandler? = nil
) async throws -> Transformer where InputSequence : Sequence, Transformer.Input == InputSequence.Element.Feature, InputSequence.Element : TemporalSequence
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

func makeTransformer() -> Transformer

Creates a default-initialized transformer suitable for incremental fitting.

Deprecated

func update&lt;InputSequence>(inout Transformer, with: InputSequence, eventHandler: EventHandler?) async throws

Does nothing since this estimator uses a pre-defined transformer.

Deprecated

