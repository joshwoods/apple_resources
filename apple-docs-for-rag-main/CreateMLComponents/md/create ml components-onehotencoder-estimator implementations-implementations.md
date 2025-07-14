

- Create ML Components
- OneHotEncoder
-  Estimator Implementations 

API Collection

# Estimator Implementations

## Topics

### Structures

struct Transformer

A transformer that encodes a category as an array of integers.

### Instance Methods

func adaptedAsSupervised&lt;Annotation>(annotationType: Annotation.Type) -> EstimatorToSupervisedAdaptor&lt;Self, Annotation>

Exposes this estimator as a supervised estimator.

func adaptedAsTemporal() -> EstimatorToTemporalAdaptor&lt;Self>

Exposes this estimator as a temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> some Estimator&lt;ComposedTransformer&lt;Self.Transformer, Other>> 

Composes this estimator with a transformer.

func appending&lt;Other>(Other) -> some SupervisedEstimator&lt;ComposedTransformer&lt;Self.Transformer, Other.Transformer>, Other.Annotation> 

Composes this estimator with a supervised estimator.

func appending&lt;Other>(Other) -> some Estimator&lt;ComposedTransformer&lt;Self.Transformer, Other.Transformer>> 

Composes this estimator with another estimator.

func appending&lt;Other>(Other) -> some SupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;TransformerToTemporalAdaptor&lt;Self.Transformer>, Other.Transformer>, Other.Annotation> 

Composes this estimator with a supervised temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> some TemporalEstimator&lt;ComposedTemporalTransformer&lt;TransformerToTemporalAdaptor&lt;Self.Transformer>, Other.Transformer>> 

Composes this estimator with a temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> some TemporalEstimator&lt;ComposedTemporalTransformer&lt;TransformerToTemporalAdaptor&lt;Self.Transformer>, Other>> 

Composes this estimator with a temporal transformer.

Deprecated

func decode(from: inout any EstimatorDecoder) throws -> Self.Transformer

Decodes a previously fitted decodable transformer.

func encode(Self.Transformer, to: inout any EstimatorEncoder) throws

Encodes a fitted encodable transformer.

func fitted&lt;S>(to: S) async throws -> Self.Transformer

func read(from: URL) throws -> Self.Transformer

Reads the encoded transformer from a file.

func write(Self.Transformer, to: URL, overwrite: Bool) throws

Writes the encoded transformer to a file.

