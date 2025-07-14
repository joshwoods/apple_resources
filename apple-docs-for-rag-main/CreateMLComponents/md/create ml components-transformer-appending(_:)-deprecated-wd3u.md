

- Create ML Components
- Transformer
-  appending(\_:) Deprecated

Instance Method

# appending(\_:)

Composes this transformer with a temporal transformer.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func appending(_ other: Other) -> ComposedTemporalTransformer, Other> where Other : TemporalTransformer, Self.Output == Other.Input
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

func appending&lt;Other, Annotation>(Other) -> some Transformer&lt;Self.Input, AnnotatedPrediction&lt;Other.Output, Annotation>> 

Composes this transformer with a prediction-only transformer.

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

