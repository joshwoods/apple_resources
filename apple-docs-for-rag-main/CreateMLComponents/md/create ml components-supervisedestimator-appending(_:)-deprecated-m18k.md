

- Create ML Components
- SupervisedEstimator
-  appending(\_:) Deprecated

Instance Method

# appending(\_:)

Composes this supervised estimator with a temporal transformer.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
@preconcurrency
func appending(_ other: Other) -> some SupervisedTemporalEstimator, Other>, Self.Annotation> where Other : TemporalTransformer, Self.Annotation : Sendable, Other.Input == Self.Transformer.Output
```

## See Also

### Appending

func appending&lt;Other>(Other) -> some SupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;TransformerToTemporalAdaptor&lt;Self.Transformer>, Other.Transformer>, Self.Annotation> 

Composes this supervised estimator with a supervised temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> some SupervisedEstimator&lt;ComposedTransformer&lt;Self.Transformer, Other.Transformer>, Self.Annotation> 

Composes this supervised estimator with another supervised estimator.

func appending&lt;Other>(Other) -> some SupervisedEstimator&lt;ComposedTransformer&lt;Self.Transformer, Other.Transformer>, Self.Annotation> 

Composes this supervised estimator with an estimator.

func appending&lt;Other>(Other) -> some SupervisedEstimator&lt;ComposedTransformer&lt;Self.Transformer, Other>, Self.Annotation> 

Composes this supervised estimator with a transformer.

func appending&lt;Other>(Other) -> some SupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;TransformerToTemporalAdaptor&lt;Self.Transformer>, Other.Transformer>, Self.Annotation> 

Composes this supervised estimator with a temporal estimator.

Deprecated

