

- Create ML Components
- FullyConnectedNetworkClassifier
-  UpdatableSupervisedEstimator Implementations 

API Collection

# UpdatableSupervisedEstimator Implementations

## Topics

### Instance Methods

func adaptedAsTemporal() -> UpdatableSupervisedEstimatorToTemporalAdaptor&lt;Self>

Exposes this supervised estimator as a temporal supervised estimator.

Deprecated

func appending&lt;Other>(Other) -> some UpdatableSupervisedEstimator&lt;ComposedTransformer&lt;Self.Transformer, Other.Transformer>, Self.Annotation> 

Composes this updatable estimator with an updatable estimator.

func appending&lt;Other>(Other) -> some UpdatableSupervisedEstimator&lt;ComposedTransformer&lt;Self.Transformer, Other>, Self.Annotation> 

Composes this updatable estimator with a transformer.

func appending&lt;Other>(Other) -> some UpdatableSupervisedEstimator&lt;ComposedTransformer&lt;Self.Transformer, Other.Transformer>, Self.Annotation> 

Composes this updatable estimator with an updatable supervised estimator.

func appending&lt;Other>(Other) -> some UpdatableSupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;TransformerToTemporalAdaptor&lt;Self.Transformer>, Other.Transformer>, Self.Annotation> 

Composes this updatable supervised estimator with an updatable supervised temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> some UpdatableSupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;TransformerToTemporalAdaptor&lt;Self.Transformer>, Other.Transformer>, Self.Annotation> 

Composes this updatable supervised estimator with an updatable temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> some UpdatableSupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;TransformerToTemporalAdaptor&lt;Self.Transformer>, Other>, Self.Annotation> 

Composes this updatable supervised estimator with a temporal transformer.

Deprecated

func decodeWithOptimizer(from: inout any EstimatorDecoder) throws -> FullyConnectedNetworkClassifier&lt;Scalar, Label>.Transformer

Decodes a previously fitted transformer with an optimizer.

func encodeWithOptimizer(FullyConnectedNetworkClassifier&lt;Scalar, Label>.Transformer, to: inout any EstimatorEncoder) throws

Encodes a fitted transformer with an optimizer.

func makeTransformer() -> FullyConnectedNetworkClassifierModel&lt;Scalar, Label>

Creates a default-initialized fully connected network classifier model suitable for incremental fitting.

func readWithOptimizer(from: URL) throws -> Self.Transformer

Reads the encoded transformer and optimizer from a file.

func update&lt;InputSequence>(inout Self.Transformer, with: InputSequence) async throws

func update&lt;InputSequence>(inout FullyConnectedNetworkClassifierModel&lt;Scalar, Label>, with: InputSequence, eventHandler: EventHandler?) async throws

Updates a fully connected network classifier model with a new sequence of examples.

func update&lt;Input>(inout Self.Transformer, with: Input, eventHandler: EventHandler?) async throws

Updates a transformer on an async sequence of examples.

func writeWithOptimizer(Self.Transformer, to: URL, overwrite: Bool) throws

Writes the encoded transformer and optimizer to a file.

