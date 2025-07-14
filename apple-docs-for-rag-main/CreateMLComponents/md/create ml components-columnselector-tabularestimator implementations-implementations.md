

- Create ML Components
- ColumnSelector
-  TabularEstimator Implementations 

API Collection

# TabularEstimator Implementations

## Topics

### Instance Methods

func adaptedAsSupervised&lt;Annotation>(annotationColumnID: ColumnID&lt;Annotation>) -> TabularEstimatorToSupervisedAdaptor&lt;Self, Annotation>

Exposes this tabular estimator as a supervised tabular estimator.

func appending&lt;Other>(Other) -> some TabularEstimator&lt;ComposedTabularTransformer&lt;Self.Transformer, Other>> 

Compose this tabular estimator with a tabular transformer.

func appending&lt;Other>(Other) -> some SupervisedTabularEstimator&lt;ComposedTabularTransformer&lt;Self.Transformer, Other.Transformer>, Other.Annotation> 

Composes this tabular estimator with a supervised tabular estimator.

func appending&lt;Other>(Other) -> some TabularEstimator&lt;ComposedTabularTransformer&lt;Self.Transformer, Other.Transformer>> 

Compose this tabular estimator with another tabular estimator.

func fitted(to: DataFrame) async throws -> Self.Transformer

func fitted(to: DataFrame) async throws -> Self.Transformer

func read(from: URL) throws -> Self.Transformer

Reads the encoded transformer from a file.

func write(Self.Transformer, to: URL, overwrite: Bool) throws

Writes the encoded transformer to a file.

