

- Create ML Components
- UpdatableSupervisedTemporalEstimator
-  update(\_:with:eventHandler:) Deprecated

Instance Method

# update(\_:with:eventHandler:)

Updates a transformer with a new sequence of examples.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func update(
    _ transformer: inout Self.Transformer,
    with input: InputSequence,
    eventHandler: EventHandler?
) async throws where InputSequence : Sequence, FeatureSequence : TemporalSequence, InputSequence.Element == AnnotatedFeature, FeatureSequence.Feature == Self.Transformer.Input
```

**Required**

## Parameters 

`transformer`  

A transformer to update.

`input`  

A sequence of examples.

`eventHandler`  

An event handler.

## See Also

### Transforming

func makeTransformer() -> Self.Transformer

Creates a default-initialized transformer suitable for incremental fitting.

**Required**

Deprecated

func update&lt;InputSequence, FeatureSequence>(inout Self.Transformer, with: InputSequence) async throwsDeprecated

