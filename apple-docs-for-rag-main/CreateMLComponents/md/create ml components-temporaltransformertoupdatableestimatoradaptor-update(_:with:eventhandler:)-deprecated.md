

- Create ML Components
- TemporalTransformerToUpdatableEstimatorAdaptor
-  update(\_:with:eventHandler:) Deprecated

Instance Method

# update(\_:with:eventHandler:)

Does nothing since this estimator uses a pre-defined transformer.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func update(
    _ transformer: inout Transformer,
    with input: InputSequence,
    eventHandler: EventHandler? = nil
) async throws where InputSequence : Sequence, Transformer.Input == InputSequence.Element.Feature, InputSequence.Element : TemporalSequence
```

## See Also

### Fitting and updating

func fitted&lt;InputSequence>(to: InputSequence, eventHandler: EventHandler?) async throws -> Transformer

Returns the pre-defined transformer.

Deprecated

func makeTransformer() -> Transformer

Creates a default-initialized transformer suitable for incremental fitting.

Deprecated

