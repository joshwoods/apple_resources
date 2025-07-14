

- Create ML Components
- Estimator
-  appending(\_:) Deprecated

Instance Method

# appending(\_:)

Composes this estimator with a temporal estimator.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func appending(_ other: Other) -> some TemporalEstimator, Other.Transformer>> where Other : TemporalEstimator, Self.Transformer.Output == Other.Transformer.Input
```

## See Also

### Appending

func appending&lt;Other>(Other) -> some TemporalEstimator&lt;ComposedTemporalTransformer&lt;TransformerToTemporalAdaptor&lt;Self.Transformer>, Other>> 

Composes this estimator with a temporal transformer.

Deprecated

func appending&lt;Other>(Other) -> some Estimator&lt;ComposedTransformer&lt;Self.Transformer, Other.Transformer>> 

Composes this estimator with another estimator.

func appending&lt;Other>(Other) -> some SupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;TransformerToTemporalAdaptor&lt;Self.Transformer>, Other.Transformer>, Other.Annotation> 

Composes this estimator with a supervised temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> some SupervisedEstimator&lt;ComposedTransformer&lt;Self.Transformer, Other.Transformer>, Other.Annotation> 

Composes this estimator with a supervised estimator.

func appending&lt;Other>(Other) -> some Estimator&lt;ComposedTransformer&lt;Self.Transformer, Other>> 

Composes this estimator with a transformer.

