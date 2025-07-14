

- Create ML Components
- SupervisedEstimatorToTemporalAdaptor
-  SupervisedTemporalEstimator Implementations 

API Collection

# SupervisedTemporalEstimator Implementations

## Topics

### Instance Methods

func appending&lt;Other>(Other) -> some SupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;Self.Transformer, TransformerToTemporalAdaptor&lt;Other.Transformer>>, Self.Annotation> 

Composes this supervised temporal estimator with a supervised estimator.

Deprecated

func appending&lt;Other>(Other) -> some SupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;Self.Transformer, Other.Transformer>, Self.Annotation> 

Composes this supervised temporal estimator with a temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> some SupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;Self.Transformer, TransformerToTemporalAdaptor&lt;Other.Transformer>>, Self.Annotation> 

Composes this supervised temporal estimator with an estimator.

Deprecated

func appending&lt;Other>(Other) -> some SupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;Self.Transformer, TransformerToTemporalAdaptor&lt;Other>>, Self.Annotation> 

Composes this supervised temporal estimator with a transformer.

Deprecated

func appending&lt;Other>(Other) -> some SupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;Self.Transformer, Other.Transformer>, Self.Annotation> 

Composes this supervised temporal estimator with another supervised temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> some SupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;Self.Transformer, Other>, Self.Annotation> 

Composes this supervised temporal estimator with a transformer.

Deprecated

func fitted&lt;InputSequence, FeatureSequence>(to: InputSequence) async throws -> Self.TransformerDeprecated

func fitted&lt;InputSequence, Validation, FeatureSequence>(to: InputSequence, validateOn: Validation) async throws -> Self.TransformerDeprecated

func read(from: URL) throws -> Self.Transformer

Reads the encoded transformer from a file.

Deprecated

func write(Self.Transformer, to: URL, overwrite: Bool) throws

Writes the encoded transformer to a file.

Deprecated

