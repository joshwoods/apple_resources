

- Create ML Components
- BoostedTreeClassifier
-  UpdatableSupervisedTabularEstimator Implementations 

API Collection

# UpdatableSupervisedTabularEstimator Implementations

## Topics

### Instance Methods

func appending&lt;Other>(Other) -> some UpdatableSupervisedTabularEstimator&lt;ComposedTabularTransformer&lt;Self.Transformer, Other>, Self.Annotation> 

Composes this supervised tabular estimator with a tabular transformer.

func appending&lt;Other>(Other) -> some UpdatableSupervisedTabularEstimator&lt;ComposedTabularTransformer&lt;Self.Transformer, Other.Transformer>, Self.Annotation> 

Composes this supervised tabular estimator with another supervised tabular estimator.

func appending&lt;Other>(Other) -> some UpdatableSupervisedTabularEstimator&lt;ComposedTabularTransformer&lt;Self.Transformer, Other.Transformer>, Self.Annotation> 

Composes this supervised tabular estimator with an updatable tabular estimator.

func decodeWithOptimizer(from: inout any EstimatorDecoder) throws -> TreeClassifierModel&lt;Label>

Reads the encoded transformer and optimizer with a decoder.

func encodeWithOptimizer(TreeClassifierModel&lt;Label>, to: inout any EstimatorEncoder) throws

Encodes the transformer and optimizer to an encoder.

func makeTransformer() -> TreeClassifierModel&lt;Label>

Creates a default-initialized transformer suitable for incremental fitting.

func readWithOptimizer(from: URL) throws -> Self.Transformer

Reads the encoded transformer and optimizer from a file.

func update(inout Self.Transformer, with: DataFrame) async throws

func update(inout TreeClassifierModel&lt;Label>, with: DataFrame, eventHandler: EventHandler?) async throws

Updates a transformer with a new sequence of examples.

func writeWithOptimizer(Self.Transformer, to: URL, overwrite: Bool) throws

Writes the encoded transformer and optimizer to a file.

