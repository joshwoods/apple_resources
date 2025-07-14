

- Create ML Components
- TemporalEstimator
-  appending(\_:) Deprecated

Instance Method

# appending(\_:)

Composes this temporal estimator with a temporal transformer.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func appending(_ other: Other) -> some TemporalEstimator> where Other : TemporalTransformer, Other.Input == Self.Transformer.Output
```

## See Also

### Appending

func appending&lt;Other>(Other) -> some SupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;Self.Transformer, Other.Transformer>, Other.Annotation> 

Composes this temporal estimator with a supervised temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> some TemporalEstimator&lt;ComposedTemporalTransformer&lt;Self.Transformer, TransformerToTemporalAdaptor&lt;Other.Transformer>>> 

Composes this temporal estimator with an estimator.

Deprecated

func appending&lt;Other>(Other) -> some TemporalEstimator&lt;ComposedTemporalTransformer&lt;Self.Transformer, TransformerToTemporalAdaptor&lt;Other>>> 

Composes this temporal estimator with a transformer.

Deprecated

func appending&lt;Other>(Other) -> some SupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;Self.Transformer, TransformerToTemporalAdaptor&lt;Other.Transformer>>, Other.Annotation> 

Composes this temporal estimator with a supervised temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> some TemporalEstimator&lt;ComposedTemporalTransformer&lt;Self.Transformer, Other.Transformer>> 

Composes this temporal estimator with another temporal estimator.

Deprecated

