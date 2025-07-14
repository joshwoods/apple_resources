

- Create ML Components
- UpdatableSupervisedTemporalEstimator
-  update(\_:with:) Deprecated

Instance Method

# update(\_:with:)

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func update(
    _ transformer: inout Self.Transformer,
    with input: InputSequence
) async throws where InputSequence : Sequence, FeatureSequence : TemporalSequence, InputSequence.Element == AnnotatedFeature, FeatureSequence.Feature == Self.Transformer.Input
```

## See Also

### Transforming

func makeTransformer() -> Self.Transformer

Creates a default-initialized transformer suitable for incremental fitting.

**Required**

Deprecated

func update&lt;InputSequence, FeatureSequence>(inout Self.Transformer, with: InputSequence, eventHandler: EventHandler?) async throws

Updates a transformer with a new sequence of examples.

**Required**

Deprecated

