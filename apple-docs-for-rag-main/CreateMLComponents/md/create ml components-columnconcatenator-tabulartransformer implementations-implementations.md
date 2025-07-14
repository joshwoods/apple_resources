

- Create ML Components
- ColumnConcatenator
-  TabularTransformer Implementations 

API Collection

# TabularTransformer Implementations

## Topics

### Instance Methods

func adaptedAsEstimator() -> TabularTransformerToEstimatorAdaptor&lt;Self>

Exposes this tabular transformer as a trivial tabular estimator.

func adaptedAsUpdatableEstimator() -> TabularTransformerToUpdatableEstimatorAdaptor&lt;Self>

Exposes this tabular transformer as an updatable tabular estimator.

func appending&lt;Other>(Other) -> PreprocessingUpdatableTabularEstimator&lt;Self, Other>

Composes this transformer with an updatable estimator.

func appending&lt;Other>(Other) -> some SupervisedTabularEstimator&lt;ComposedTabularTransformer&lt;Self, Other.Transformer>, Other.Annotation> 

Composes this transformer with a supervised tabular estimator.

func appending&lt;Other>(Other) -> ComposedTabularTransformer&lt;Self, Other>

Composes this tabular transformer with another tabular transformer.

func appending&lt;Other>(Other) -> some TabularEstimator&lt;ComposedTabularTransformer&lt;Self, Other.Transformer>> 

Compose this tabular transformer with a tabular estimator.

func appending&lt;Other>(Other) -> PreprocessingTabularEstimator&lt;Self, Other>

Composes this transformer with an estimator.

func appending&lt;Other>(Other) -> PreprocessingSupervisedTabularEstimator&lt;Self, Other>

Composes this transformer with a supervised tabular estimator.

func appending&lt;Other>(Other) -> PreprocessingUpdatableSupervisedTabularEstimator&lt;Self, Other>

Composes this transformer with an updatable supervised estimator.

func callAsFunction(DataFrame, eventHandler: EventHandler?) async throws -> DataFrame

Performs the transformation on a single input.

func export(to: URL) throws

Exports this transformer as a CoreML model.

func export(to: URL, metadata: ModelMetadata) throws

Exports this tabular transformer as a CoreML model with userInfo.

