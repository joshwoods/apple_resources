

- Create ML Components
- Estimator
-  appending(\_:) 

Instance Method

# appending(\_:)

Composes this estimator with another estimator.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func appending(_ other: Other) -> some Estimator> where Other : Estimator, Self.Transformer.Output == Other.Transformer.Input
```

## See Also

### Appending

func appending&lt;Other>(Other) -> some TemporalEstimator&lt;ComposedTemporalTransformer&lt;TransformerToTemporalAdaptor&lt;Self.Transformer>, Other>> 

Composes this estimator with a temporal transformer.

Deprecated

func appending&lt;Other>(Other) -> some SupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;TransformerToTemporalAdaptor&lt;Self.Transformer>, Other.Transformer>, Other.Annotation> 

Composes this estimator with a supervised temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> some SupervisedEstimator&lt;ComposedTransformer&lt;Self.Transformer, Other.Transformer>, Other.Annotation> 

Composes this estimator with a supervised estimator.

func appending&lt;Other>(Other) -> some Estimator&lt;ComposedTransformer&lt;Self.Transformer, Other>> 

Composes this estimator with a transformer.

func appending&lt;Other>(Other) -> some TemporalEstimator&lt;ComposedTemporalTransformer&lt;TransformerToTemporalAdaptor&lt;Self.Transformer>, Other.Transformer>> 

Composes this estimator with a temporal estimator.

Deprecated

