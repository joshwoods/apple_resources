

- Create ML Components
- AudioReader
-  Transformer Implementations 

API Collection

# Transformer Implementations

## Topics

### Instance Methods

func adaptedAsAnnotatedFeatureTransformer&lt;Annotation>(annotationType: Annotation.Type) -> some Transformer&lt;AnnotatedFeature&lt;Self.Input, Annotation>, AnnotatedFeature&lt;Self.Output, Annotation>> 

Returns an annotated-feature transformer that transforms the features using this transformer while leaving the annotations unchanged.

func adaptedAsAnnotatedPredictionTransformer&lt;Annotation>(annotationType: Annotation.Type) -> some Transformer&lt;AnnotatedPrediction&lt;Self.Input, Annotation>, AnnotatedPrediction&lt;Self.Output, Annotation>> 

Returns an annotated-prediction transformer that transforms the predictions using this transformer while leaving the annotations unchanged.

func adaptedAsEstimator() -> TransformerToEstimatorAdaptor&lt;Self>

Exposes this transformer as a trivial estimator.

func adaptedAsRandomTransformer() -> some RandomTransformer&lt;Self.Input, Self.Output> 

Returns a random transformer wrapping a transformer.

func adaptedAsTemporal() -> TransformerToTemporalAdaptor&lt;Self>

Exposes this transformer as a temporal transformer.

Deprecated

func adaptedAsUpdatableEstimator() -> TransformerToUpdatableEstimatorAdaptor&lt;Self>

Exposes this transformer as a trivial estimator.

func appending&lt;Other>(Other) -> ComposedTemporalTransformer&lt;TemporalAdaptor&lt;Self>, Other>

Composes this transformer with a temporal transformer.

func appending&lt;Other, Annotation>(Other) -> some Transformer&lt;Self.Input, AnnotatedFeature&lt;Other.Output, Annotation>> 

Composes this transformer with a feature-only transformer.

func appending&lt;Other>(Other) -> ComposedTemporalTransformer&lt;TransformerToTemporalAdaptor&lt;Self>, Other>

Composes this transformer with a temporal transformer.

Deprecated

func appending&lt;Other>(Other) -> PreprocessingUpdatableEstimator&lt;Self, Other>

Composes this transformer with an updatable estimator.

func appending&lt;Other>(Other) -> PreprocessingUpdatableSupervisedTemporalEstimator&lt;TransformerToTemporalAdaptor&lt;Self>, Other>

Composes this transformer with an updatable supervised temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> PreprocessingTemporalEstimator&lt;TransformerToTemporalAdaptor&lt;Self>, Other>

Composes this transformer with a temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> PreprocessingSupervisedEstimator&lt;Self, Other>

Composes this transformer with a supervised estimator.

func appending&lt;Other>(Other) -> PreprocessingUpdatableSupervisedEstimator&lt;Self, Other>

Composes this transformer with an updatable supervised estimator.

func appending&lt;Other, Annotation>(Other) -> some Transformer&lt;AnnotatedFeature&lt;Self.Input, Annotation>, Other.Output> 

Composes this transformer with an annotated-feature transformer.

func appending&lt;Other>(Other) -> PreprocessingSupervisedTemporalEstimator&lt;TransformerToTemporalAdaptor&lt;Self>, Other>

Composes this transformer with a supervised temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> PreprocessingEstimator&lt;Self, Other>

Composes this transformer with an estimator.

func appending&lt;Other>(Other) -> ComposedTransformer&lt;Self, Other>

Composes this transformer with another transformer.

func appending&lt;Other>(Other) -> PreprocessingUpdatableTemporalEstimator&lt;TransformerToTemporalAdaptor&lt;Self>, Other>

Composes this transformer with an updatable temporal estimator.

Deprecated

func appending&lt;Other, Annotation>(Other) -> some Transformer&lt;AnnotatedPrediction&lt;Self.Input, Annotation>, Other.Output> 

Composes this transformer with an annotated-feature transformer.

func appending&lt;Other, Annotation>(Other) -> some Transformer&lt;Self.Input, AnnotatedPrediction&lt;Other.Output, Annotation>> 

Composes this transformer with a prediction-only transformer.

func callAsFunction(Self.Input, eventHandler: EventHandler?) async throws -> Self.Output

Performs the transformation on a single input.

func callAsFunction&lt;S>(S, eventHandler: EventHandler?) async throws -> [Self.Output]

Performs the transformation on a sequence of inputs.

func export(to: URL) throws

Exports this transformer as a CoreML model.

func export(to: URL, metadata: ModelMetadata) throws

Exports this transformer as a CoreML model with userInfo.

func prediction&lt;Label>(from: Self.Input) async throws -> ClassificationDistribution&lt;Label>

Performs a prediction from a single input.

func prediction&lt;S, Label>(from: S) async throws -> [ClassificationDistribution&lt;Label>]

Performs a prediction from a sequence of inputs.

func prediction&lt;S, Annotation>(from: S, eventHandler: EventHandler?) async throws -> [AnnotatedPrediction&lt;Self.Output, Annotation>]

Performs a prediction on a sequence of annotated inputs.

