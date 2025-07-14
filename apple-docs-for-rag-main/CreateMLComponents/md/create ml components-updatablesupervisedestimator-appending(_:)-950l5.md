

- Create ML Components
- UpdatableSupervisedEstimator
-  appending(\_:) 

Instance Method

# appending(\_:)

Composes this updatable estimator with a transformer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func appending(_ other: Other) -> some UpdatableSupervisedEstimator, Self.Annotation> where Other : Transformer, Other.Input == Self.Transformer.Output
```

## See Also

### Appending

func appending&lt;Other>(Other) -> some UpdatableSupervisedEstimator&lt;ComposedTransformer&lt;Self.Transformer, Other.Transformer>, Self.Annotation> 

Composes this updatable estimator with an updatable estimator.

func appending&lt;Other>(Other) -> some UpdatableSupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;TransformerToTemporalAdaptor&lt;Self.Transformer>, Other.Transformer>, Self.Annotation> 

Composes this updatable supervised estimator with an updatable temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> some UpdatableSupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;TransformerToTemporalAdaptor&lt;Self.Transformer>, Other>, Self.Annotation> 

Composes this updatable supervised estimator with a temporal transformer.

Deprecated

func appending&lt;Other>(Other) -> some UpdatableSupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;TransformerToTemporalAdaptor&lt;Self.Transformer>, Other.Transformer>, Self.Annotation> 

Composes this updatable supervised estimator with an updatable supervised temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> some UpdatableSupervisedEstimator&lt;ComposedTransformer&lt;Self.Transformer, Other.Transformer>, Self.Annotation> 

Composes this updatable estimator with an updatable supervised estimator.

