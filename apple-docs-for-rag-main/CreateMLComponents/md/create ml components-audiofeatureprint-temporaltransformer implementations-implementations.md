

- Create ML Components
- AudioFeaturePrint
-  TemporalTransformer Implementations 

API Collection

# TemporalTransformer Implementations

## Topics

### Instance Methods

func adaptedAsEstimator() -> TemporalTransformerToEstimatorAdaptor&lt;Self>

Exposes this temporal transformer as a trivial temporal estimator.

Deprecated

func adaptedAsUpdatableEstimator() -> TemporalTransformerToUpdatableEstimatorAdaptor&lt;Self>

Exposes this temporal transformer as a trivial temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> PreprocessingTemporalEstimator&lt;Self, EstimatorToTemporalAdaptor&lt;Other>>

Composes this temporal transformer with an estimator.

Deprecated

func appending&lt;Other>(Other) -> PreprocessingUpdatableTemporalEstimator&lt;Self, Other>

Composes this temporal transformer with an updatable temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> PreprocessingUpdatableSupervisedTemporalEstimator&lt;Self, Other>

Composes this transformer with an updatable supervised temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> PreprocessingUpdatableSupervisedTemporalEstimator&lt;Self, UpdatableSupervisedEstimatorToTemporalAdaptor&lt;Other>>

Composes this transformer with an updatable supervised temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> ComposedTemporalTransformer&lt;Self, Other>

Composes this temporal transformer with another temporal transformer.

func appending&lt;Other>(Other) -> ComposedTemporalTransformer&lt;Self, TransformerToTemporalAdaptor&lt;Other>>

Composes this temporal transformer with a transformer.

Deprecated

func appending&lt;Other>(Other) -> PreprocessingTemporalEstimator&lt;Self, Other>

Composes this temporal transformer with a temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> ComposedTemporalTransformer&lt;Self, TemporalAdaptor&lt;Other>>

Composes this temporal transformer with a transformer.

func appending&lt;Other>(Other) -> PreprocessingSupervisedTemporalEstimator&lt;Self, Other>

Composes this transformer with a supervised temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> PreprocessingUpdatableTemporalEstimator&lt;Self, UpdatableEstimatorToTemporalAdaptor&lt;Other>>

Composes this temporal transformer with an updatable estimator.

Deprecated

func appending&lt;Other>(Other) -> PreprocessingSupervisedTemporalEstimator&lt;Self, SupervisedEstimatorToTemporalAdaptor&lt;Other>>

Composes this transformer with a supervised temporal estimator.

Deprecated

func applied&lt;S>(to: S, eventHandler: EventHandler?) async throws -> [Self.OutputSequence]

Performs the transformation on a sequence of input sequences.

func applied&lt;S, TS, Annotation>(to: S, eventHandler: EventHandler?) async throws -> [AnnotatedFeature&lt;Self.OutputSequence, Annotation>]

Performs the transformation on a sequence of annotated input sequences.

func callAsFunction&lt;S>(S, eventHandler: EventHandler?) async throws -> Self.OutputSequence

Performs the transformation on an input sequence.

func callAsFunction&lt;S>(to: S, eventHandler: EventHandler?) async throws -> [Self.OutputSequence]

Performs the transformation on a sequence of inputs.

func export(to: URL) throws

Exports this temporal transformer as a CoreML model.

func export(to: URL, metadata: ModelMetadata) throws

Exports this temporal transformer as a CoreML model with user-supplied metadata.

func prediction&lt;S, Label>(from: S) async throws -> Self.OutputSequence

Performs a prediction on a single input.

