

- Create ML Components
- UpdatableTemporalEstimatorToSupervisedAdaptor
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

