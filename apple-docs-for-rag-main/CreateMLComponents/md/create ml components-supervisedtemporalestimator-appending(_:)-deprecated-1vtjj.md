

- Create ML Components
- SupervisedTemporalEstimator
-  appending(\_:) Deprecated

Instance Method

# appending(\_:)

Composes this supervised temporal estimator with a supervised estimator.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func appending(_ other: Other) -> some SupervisedTemporalEstimator>, Self.Annotation> where Other : SupervisedEstimator, Self.Annotation == Other.Annotation, Self.Transformer.Output == Other.Transformer.Input
```

## See Also

### Appending

func appending&lt;Other>(Other) -> some SupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;Self.Transformer, Other>, Self.Annotation> 

Composes this supervised temporal estimator with a transformer.

Deprecated

func appending&lt;Other>(Other) -> some SupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;Self.Transformer, Other.Transformer>, Self.Annotation> 

Composes this supervised temporal estimator with another supervised temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> some SupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;Self.Transformer, Other.Transformer>, Self.Annotation> 

Composes this supervised temporal estimator with a temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> some SupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;Self.Transformer, TransformerToTemporalAdaptor&lt;Other.Transformer>>, Self.Annotation> 

Composes this supervised temporal estimator with an estimator.

Deprecated

func appending&lt;Other>(Other) -> some SupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;Self.Transformer, TransformerToTemporalAdaptor&lt;Other>>, Self.Annotation> 

Composes this supervised temporal estimator with a transformer.

Deprecated

