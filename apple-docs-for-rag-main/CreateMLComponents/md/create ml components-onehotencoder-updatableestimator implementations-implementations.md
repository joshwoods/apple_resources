

- Create ML Components
- OneHotEncoder
-  UpdatableEstimator Implementations 

API Collection

# UpdatableEstimator Implementations

## Topics

### Instance Methods

func adaptedAsSupervised&lt;Annotation>(annotationType: Annotation.Type) -> UpdatableEstimatorToSupervisedAdaptor&lt;Self, Annotation>

Exposes this estimator as a supervised estimator.

func adaptedAsTemporal() -> UpdatableEstimatorToTemporalAdaptor&lt;Self>

Exposes this estimator as a temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> some UpdatableEstimator&lt;ComposedTransformer&lt;Self.Transformer, Other>> 

Composes this updatable estimator with a transformer.

func appending&lt;Other>(Other) -> some UpdatableTemporalEstimator&lt;ComposedTemporalTransformer&lt;TransformerToTemporalAdaptor&lt;Self.Transformer>, Other.Transformer>> 

Composes this updatable estimator with an updatable temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> some UpdatableSupervisedEstimator&lt;ComposedTransformer&lt;Self.Transformer, Other.Transformer>, Other.Annotation> 

Composes this updatable estimator with an updatable supervised estimator.

func appending&lt;Other>(Other) -> some UpdatableTemporalEstimator&lt;ComposedTemporalTransformer&lt;TransformerToTemporalAdaptor&lt;Self.Transformer>, Other>> 

Composes this updatable estimator with a temporal transformer.

Deprecated

func appending&lt;Other>(Other) -> some UpdatableSupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;TransformerToTemporalAdaptor&lt;Self.Transformer>, Other.Transformer>, Other.Annotation> 

Composes this updatable estimator with an updatable supervised temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> some UpdatableEstimator&lt;ComposedTransformer&lt;Self.Transformer, Other.Transformer>> 

Composes this updatable estimator with another updatable estimator.

func decodeWithOptimizer(from: inout any EstimatorDecoder) throws -> OneHotEncoder&lt;Category>.Transformer

Reads the encoded transformer with a decoder.

func encodeWithOptimizer(OneHotEncoder&lt;Category>.Transformer, to: inout any EstimatorEncoder) throws

Encodes the transformer to an encoder.

func makeTransformer() -> OneHotEncoder&lt;Category>.Transformer

Creates a default-initialized transformer suitable for incremental fitting.

func update&lt;InputSequence>(inout Self.Transformer, with: InputSequence) async throws

func update(inout OneHotEncoder&lt;Category>.Transformer, with: some Sequence&lt;Optional&lt;Category>>, eventHandler: EventHandler?) throws

Updates a transformer with a new sequence of examples.

