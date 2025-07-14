

- Create ML Components
- Transformer
-  appending(\_:) 

Instance Method

# appending(\_:)

Composes this transformer with a prediction-only transformer.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
func appending(_ other: Other) -> some Transformer> where Other : Transformer, Self.Output == AnnotatedPrediction
```

## See Also

### Appending

func appending&lt;Other>(Other) -> PreprocessingSupervisedTemporalEstimator&lt;TransformerToTemporalAdaptor&lt;Self>, Other>

Composes this transformer with a supervised temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> PreprocessingTemporalEstimator&lt;TransformerToTemporalAdaptor&lt;Self>, Other>

Composes this transformer with a temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> PreprocessingUpdatableSupervisedTemporalEstimator&lt;TransformerToTemporalAdaptor&lt;Self>, Other>

Composes this transformer with an updatable supervised temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> PreprocessingUpdatableEstimator&lt;Self, Other>

Composes this transformer with an updatable estimator.

func appending&lt;Other, Annotation>(Other) -> some Transformer&lt;AnnotatedFeature&lt;Self.Input, Annotation>, Other.Output> 

Composes this transformer with an annotated-feature transformer.

func appending&lt;Other>(Other) -> ComposedTransformer&lt;Self, Other>

Composes this transformer with another transformer.

func appending&lt;Other>(Other) -> PreprocessingUpdatableSupervisedEstimator&lt;Self, Other>

Composes this transformer with an updatable supervised estimator.

func appending&lt;Other>(Other) -> PreprocessingEstimator&lt;Self, Other>

Composes this transformer with an estimator.

func appending&lt;Other, Annotation>(Other) -> some Transformer&lt;Self.Input, AnnotatedFeature&lt;Other.Output, Annotation>> 

Composes this transformer with a feature-only transformer.

func appending&lt;Other, Annotation>(Other) -> some Transformer&lt;AnnotatedPrediction&lt;Self.Input, Annotation>, Other.Output> 

Composes this transformer with an annotated-feature transformer.

func appending&lt;Other>(Other) -> PreprocessingSupervisedEstimator&lt;Self, Other>

Composes this transformer with a supervised estimator.

func appending&lt;Other>(Other) -> PreprocessingUpdatableTemporalEstimator&lt;TransformerToTemporalAdaptor&lt;Self>, Other>

Composes this transformer with an updatable temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> ComposedTemporalTransformer&lt;TransformerToTemporalAdaptor&lt;Self>, Other>

Composes this transformer with a temporal transformer.

Deprecated

