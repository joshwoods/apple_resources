

- Create ML Components
- MultivariateLinearRegressor
-  UpdatableSupervisedEstimator Implementations 

API Collection

# UpdatableSupervisedEstimator Implementations

## Topics

### Instance Methods

func adaptedAsTemporal() -> UpdatableSupervisedEstimatorToTemporalAdaptor&lt;Self>

Exposes this supervised estimator as a temporal supervised estimator.

Deprecated

func appending&lt;Other>(Other) -> some UpdatableSupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;TransformerToTemporalAdaptor&lt;Self.Transformer>, Other.Transformer>, Self.Annotation> 

Composes this updatable supervised estimator with an updatable temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> some UpdatableSupervisedEstimator&lt;ComposedTransformer&lt;Self.Transformer, Other>, Self.Annotation> 

Composes this updatable estimator with a transformer.

func appending&lt;Other>(Other) -> some UpdatableSupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;TransformerToTemporalAdaptor&lt;Self.Transformer>, Other>, Self.Annotation> 

Composes this updatable supervised estimator with a temporal transformer.

Deprecated

func appending&lt;Other>(Other) -> some UpdatableSupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;TransformerToTemporalAdaptor&lt;Self.Transformer>, Other.Transformer>, Self.Annotation> 

Composes this updatable supervised estimator with an updatable supervised temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> some UpdatableSupervisedEstimator&lt;ComposedTransformer&lt;Self.Transformer, Other.Transformer>, Self.Annotation> 

Composes this updatable estimator with an updatable supervised estimator.

func appending&lt;Other>(Other) -> some UpdatableSupervisedEstimator&lt;ComposedTransformer&lt;Self.Transformer, Other.Transformer>, Self.Annotation> 

Composes this updatable estimator with an updatable estimator.

func decodeWithOptimizer(from: inout any EstimatorDecoder) throws -> MultivariateLinearRegressor&lt;Scalar>.Model

Reads the encoded model and optimizer with a decoder.

func encodeWithOptimizer(MultivariateLinearRegressor&lt;Scalar>.Model, to: inout any EstimatorEncoder) throws

Encodes the model and optimizer to an encoder.

func makeTransformer() -> MultivariateLinearRegressor&lt;Scalar>.Model

Creates a default-initialized model suitable for incremental fitting.

func readWithOptimizer(from: URL) throws -> Self.Transformer

Reads the encoded transformer and optimizer from a file.

func update(inout MultivariateLinearRegressor&lt;Scalar>.Model, with: some Sequence&lt;AnnotatedFeature&lt;MLShapedArray&lt;Scalar>, MLShapedArray&lt;Scalar>>>, eventHandler: EventHandler?) async throws

Updates a model with a new sequence of examples.

func update&lt;Input>(inout Self.Transformer, with: Input, eventHandler: EventHandler?) async throws

Updates a transformer on an async sequence of examples.

func writeWithOptimizer(Self.Transformer, to: URL, overwrite: Bool) throws

Writes the encoded transformer and optimizer to a file.

