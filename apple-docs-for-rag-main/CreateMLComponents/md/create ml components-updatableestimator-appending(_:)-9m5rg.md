

- Create ML Components
- UpdatableEstimator
-  appending(\_:) 

Instance Method

# appending(\_:)

Composes this updatable estimator with an updatable supervised estimator.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func appending(_ other: Other) -> some UpdatableSupervisedEstimator, Other.Annotation> where Other : UpdatableSupervisedEstimator, Self.Transformer.Output == Other.Transformer.Input
```

## See Also

### Appending

func appending&lt;Other>(Other) -> some UpdatableEstimator&lt;ComposedTransformer&lt;Self.Transformer, Other>> 

Composes this updatable estimator with a transformer.

func appending&lt;Other>(Other) -> some UpdatableTemporalEstimator&lt;ComposedTemporalTransformer&lt;TransformerToTemporalAdaptor&lt;Self.Transformer>, Other.Transformer>> 

Composes this updatable estimator with an updatable temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> some UpdatableTemporalEstimator&lt;ComposedTemporalTransformer&lt;TransformerToTemporalAdaptor&lt;Self.Transformer>, Other>> 

Composes this updatable estimator with a temporal transformer.

Deprecated

func appending&lt;Other>(Other) -> some UpdatableSupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;TransformerToTemporalAdaptor&lt;Self.Transformer>, Other.Transformer>, Other.Annotation> 

Composes this updatable estimator with an updatable supervised temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> some UpdatableEstimator&lt;ComposedTransformer&lt;Self.Transformer, Other.Transformer>> 

Composes this updatable estimator with another updatable estimator.

