

- Create ML Components
- TemporalTransformerToEstimatorAdaptor
-  fitted(to:) Deprecated

Instance Method

# fitted(to:)

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func fitted(to input: InputSequence) async throws -> Self.Transformer where InputSequence : Sequence, InputSequence.Element : TemporalSequence, Self.Transformer.Input == InputSequence.Element.Feature
```

