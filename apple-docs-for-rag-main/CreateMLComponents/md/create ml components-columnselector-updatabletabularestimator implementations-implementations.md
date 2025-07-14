

- Create ML Components
- ColumnSelector
-  UpdatableTabularEstimator Implementations 

API Collection

# UpdatableTabularEstimator Implementations

## Topics

### Instance Methods

func adaptedAsSupervised&lt;Annotation>(annotationColumnID: ColumnID&lt;Annotation>) -> UpdatableTabularEstimatorToSupervisedAdaptor&lt;Self, Annotation>

Exposes this updatable tabular estimator as a supervised tabular estimator.

func appending&lt;Other>(Other) -> some UpdatableTabularEstimator&lt;ComposedTabularTransformer&lt;Self.Transformer, Other>> 

Composes this updatable tabular estimator with a tabular transformer.

func appending&lt;Other>(Other) -> some UpdatableSupervisedTabularEstimator&lt;ComposedTabularTransformer&lt;Self.Transformer, Other.Transformer>, Other.Annotation> 

Composes this updatable tabular estimator with an updatable supervised tabular estimator.

func appending&lt;Other>(Other) -> some UpdatableTabularEstimator&lt;ComposedTabularTransformer&lt;Self.Transformer, Other.Transformer>> 

Composes this updatable tabular estimator with another updatable tabular estimator.

func decodeWithOptimizer(from: inout any EstimatorDecoder) throws -> ColumnSelector&lt;Estimator, UnwrappedInput>.Transformer

Reads the encoded transformer and optimizer with a decoder.

func encodeWithOptimizer(ColumnSelector&lt;Estimator, UnwrappedInput>.Transformer, to: inout any EstimatorEncoder) throws

Encodes the transformer and optimizer to an encoder.

func makeTransformer() -> ColumnSelectorTransformer&lt;Estimator.Transformer, UnwrappedInput>

Creates a default-initialized transformer suitable for incremental fitting.

func update(inout Self.Transformer, with: DataFrame) async throws

func update(inout ColumnSelector&lt;Estimator, UnwrappedInput>.Transformer, with: DataFrame, eventHandler: EventHandler?) async throws

Updates a transformer with a new sequence of examples.

