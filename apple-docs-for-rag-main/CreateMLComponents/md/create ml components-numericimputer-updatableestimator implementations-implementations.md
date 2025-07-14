

- Create ML Components
- NumericImputer
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

func appending&lt;Other>(Other) -> some UpdatableEstimator&lt;ComposedTransformer&lt;Self.Transformer, Other.Transformer>> 

Composes this updatable estimator with another updatable estimator.

func appending&lt;Other>(Other) -> some UpdatableEstimator&lt;ComposedTransformer&lt;Self.Transformer, Other>> 

Composes this updatable estimator with a transformer.

func appending&lt;Other>(Other) -> some UpdatableSupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;TransformerToTemporalAdaptor&lt;Self.Transformer>, Other.Transformer>, Other.Annotation> 

Composes this updatable estimator with an updatable supervised temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> some UpdatableTemporalEstimator&lt;ComposedTemporalTransformer&lt;TransformerToTemporalAdaptor&lt;Self.Transformer>, Other>> 

Composes this updatable estimator with a temporal transformer.

Deprecated

func appending&lt;Other>(Other) -> some UpdatableTemporalEstimator&lt;ComposedTemporalTransformer&lt;TransformerToTemporalAdaptor&lt;Self.Transformer>, Other.Transformer>> 

Composes this updatable estimator with an updatable temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> some UpdatableSupervisedEstimator&lt;ComposedTransformer&lt;Self.Transformer, Other.Transformer>, Other.Annotation> 

Composes this updatable estimator with an updatable supervised estimator.

func decodeWithOptimizer(from: inout any EstimatorDecoder) throws -> NumericImputer&lt;Element>.Transformer

Reads the encoded transformer with a decoder.

func encodeWithOptimizer(NumericImputer&lt;Element>.Transformer, to: inout any EstimatorEncoder) throws

Encodes the transformer to an encoder.

func makeTransformer() -> NumericImputer&lt;Element>.Transformer

Creates a default-initialized impute transformer suitable for incremental fitting.

func update&lt;InputSequence>(inout Self.Transformer, with: InputSequence) async throws

func update(inout ImputeTransformer&lt;Element>, with: some Sequence&lt;Optional&lt;Element>>, eventHandler: EventHandler?) throws

Updates an impute transformer with a new sequence of examples.

