

- Create ML Components
- UpdatableEstimator
-  appending(\_:) Deprecated

Instance Method

# appending(\_:)

Composes this updatable estimator with an updatable temporal estimator.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func appending(_ other: Other) -> some UpdatableTemporalEstimator, Other.Transformer>> where Other : UpdatableTemporalEstimator, Self.Transformer.Output == Other.Transformer.Input
```

## See Also

### Appending

func appending&lt;Other>(Other) -> some UpdatableEstimator&lt;ComposedTransformer&lt;Self.Transformer, Other>> 

Composes this updatable estimator with a transformer.

func appending&lt;Other>(Other) -> some UpdatableTemporalEstimator&lt;ComposedTemporalTransformer&lt;TransformerToTemporalAdaptor&lt;Self.Transformer>, Other>> 

Composes this updatable estimator with a temporal transformer.

Deprecated

func appending&lt;Other>(Other) -> some UpdatableSupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;TransformerToTemporalAdaptor&lt;Self.Transformer>, Other.Transformer>, Other.Annotation> 

Composes this updatable estimator with an updatable supervised temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> some UpdatableEstimator&lt;ComposedTransformer&lt;Self.Transformer, Other.Transformer>> 

Composes this updatable estimator with another updatable estimator.

func appending&lt;Other>(Other) -> some UpdatableSupervisedEstimator&lt;ComposedTransformer&lt;Self.Transformer, Other.Transformer>, Other.Annotation> 

Composes this updatable estimator with an updatable supervised estimator.

