

- Create ML Components
- PreprocessingUpdatableSupervisedTemporalEstimator
-  fitted(to:validateOn:) Deprecated

Instance Method

# fitted(to:validateOn:)

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func fitted(
    to input: InputSequence,
    validateOn validation: Validation
) async throws -> Self.Transformer where InputSequence : Sequence, Validation : Sequence, FeatureSequence : TemporalSequence, InputSequence.Element == AnnotatedFeature, Validation.Element == AnnotatedFeature, FeatureSequence.Feature == Self.Transformer.Input
```

