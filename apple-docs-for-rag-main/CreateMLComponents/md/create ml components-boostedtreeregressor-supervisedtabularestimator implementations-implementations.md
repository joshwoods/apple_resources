

- Create ML Components
- BoostedTreeRegressor
-  SupervisedTabularEstimator Implementations 

API Collection

# SupervisedTabularEstimator Implementations

## Topics

### Instance Methods

func appending&lt;Other>(Other) -> some SupervisedTabularEstimator&lt;ComposedTabularTransformer&lt;Self.Transformer, Other.Transformer>, Self.Annotation> 

Composes this supervised tabular estimator with another supervised tabular estimator.

func appending&lt;Other>(Other) -> some SupervisedTabularEstimator&lt;ComposedTabularTransformer&lt;Self.Transformer, Other.Transformer>, Self.Annotation> 

Composes this tabular supervised estimator with a tabular estimator.

func appending&lt;Other>(Other) -> some SupervisedTabularEstimator&lt;ComposedTabularTransformer&lt;Self.Transformer, Other>, Self.Annotation> 

Composes this supervised tabular estimator with a tabular transformer.

func fitted(to: DataFrame, validateOn: DataFrame?) async throws -> Self.Transformer

func read(from: URL) throws -> Self.Transformer

Reads the encoded transformer from a file.

func write(Self.Transformer, to: URL, overwrite: Bool) throws

Writes the encoded transformer to a file.

