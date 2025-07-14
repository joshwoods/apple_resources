

- Create ML Components
- TemporalTransformerToUpdatableEstimatorAdaptor
-  TemporalEstimator Implementations 

API Collection

# TemporalEstimator Implementations

## Topics

### Instance Methods

func adaptedAsSupervised&lt;Annotation>(annotationType: Annotation.Type) -> TemporalEstimatorToSupervisedAdaptor&lt;Self, Annotation>

Exposes this temporal estimator as a supervised temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> some SupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;Self.Transformer, TransformerToTemporalAdaptor&lt;Other.Transformer>>, Other.Annotation> 

Composes this temporal estimator with a supervised temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> some TemporalEstimator&lt;ComposedTemporalTransformer&lt;Self.Transformer, TransformerToTemporalAdaptor&lt;Other>>> 

Composes this temporal estimator with a transformer.

Deprecated

func appending&lt;Other>(Other) -> some SupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;Self.Transformer, Other.Transformer>, Other.Annotation> 

Composes this temporal estimator with a supervised temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> some TemporalEstimator&lt;ComposedTemporalTransformer&lt;Self.Transformer, Other.Transformer>> 

Composes this temporal estimator with another temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> some TemporalEstimator&lt;ComposedTemporalTransformer&lt;Self.Transformer, TransformerToTemporalAdaptor&lt;Other.Transformer>>> 

Composes this temporal estimator with an estimator.

Deprecated

func appending&lt;Other>(Other) -> some TemporalEstimator&lt;ComposedTemporalTransformer&lt;Self.Transformer, Other>> 

Composes this temporal estimator with a temporal transformer.

Deprecated

func fitted&lt;InputSequence>(to: InputSequence) async throws -> Self.TransformerDeprecated

func read(from: URL) throws -> Self.Transformer

Reads the encoded transformer from a file.

Deprecated

func write(Self.Transformer, to: URL, overwrite: Bool) throws

Writes the encoded transformer to a file.

Deprecated

