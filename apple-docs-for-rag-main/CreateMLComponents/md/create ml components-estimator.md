

- Create ML Components
-  Estimator 

Protocol

# Estimator

An estimator that creates a transformer by fitting to a data set.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
protocol Estimator
```

## Topics

### Getting the properties

associatedtype Transformer : Transformer

The transformer type created by this estimator.

**Required**

### Appending

func appending&lt;Other>(Other) -> some TemporalEstimator&lt;ComposedTemporalTransformer&lt;TransformerToTemporalAdaptor&lt;Self.Transformer>, Other>> 

Composes this estimator with a temporal transformer.

Deprecated

func appending&lt;Other>(Other) -> some Estimator&lt;ComposedTransformer&lt;Self.Transformer, Other.Transformer>> 

Composes this estimator with another estimator.

func appending&lt;Other>(Other) -> some SupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;TransformerToTemporalAdaptor&lt;Self.Transformer>, Other.Transformer>, Other.Annotation> 

Composes this estimator with a supervised temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> some SupervisedEstimator&lt;ComposedTransformer&lt;Self.Transformer, Other.Transformer>, Other.Annotation> 

Composes this estimator with a supervised estimator.

func appending&lt;Other>(Other) -> some Estimator&lt;ComposedTransformer&lt;Self.Transformer, Other>> 

Composes this estimator with a transformer.

func appending&lt;Other>(Other) -> some TemporalEstimator&lt;ComposedTemporalTransformer&lt;TransformerToTemporalAdaptor&lt;Self.Transformer>, Other.Transformer>> 

Composes this estimator with a temporal estimator.

Deprecated

### Encoding and decoding

func encode(Self.Transformer, to: inout any EstimatorEncoder) throws

Encodes a fitted transformer.

**Required** Default implementation provided.

func decode(from: inout any EstimatorDecoder) throws -> Self.Transformer

Decodes a previously fitted transformer.

**Required** Default implementation provided.

### Reading and writing

func read(from: URL) throws -> Self.Transformer

Reads the encoded transformer from a file.

func write(Self.Transformer, to: URL, overwrite: Bool) throws

Writes the encoded transformer to a file.

### Fitting and adapting

func adaptedAsSupervised&lt;Annotation>(annotationType: Annotation.Type) -> EstimatorToSupervisedAdaptor&lt;Self, Annotation>

Exposes this estimator as a supervised estimator.

func adaptedAsTemporal() -> EstimatorToTemporalAdaptor&lt;Self>

Exposes this estimator as a temporal estimator.

Deprecated

func fitted&lt;S>(to: S, eventHandler: EventHandler?) async throws -> Self.Transformer

Fits a transformer to a sequence of examples.

**Required**

func fitted&lt;S>(to: S) async throws -> Self.Transformer

## Relationships

### Inherited By

- UpdatableEstimator

### Conforming Types

- CategoricalImputer
- MaxAbsScaler
- MinMaxScaler
- NormalizationScaler
- NumericImputer
- OneHotEncoder

  Conforms when `Category` conforms to `Comparable`, `Decodable`, `Encodable`, and `Hashable`.

- OrdinalEncoder
- PreprocessingEstimator
- PreprocessingUpdatableEstimator
- RobustScaler
- StandardScaler
- TransformerToEstimatorAdaptor
- TransformerToUpdatableEstimatorAdaptor

## See Also

### Protocols

protocol Transformer

A transformer that takes an input and produces an output.

protocol TemporalTransformer

A transformer that takes an asynchronous input sequence of temporal features and produces an asynchronous output sequence.

protocol RandomTransformer

A transformer that takes an input and a random number generator and produces a randomized output.

protocol TemporalEstimator

An estimator that creates a transformer by fitting to a sequence of temporal features.

Deprecated

protocol SupervisedEstimator

An estimator that creates a transformer by fitting to a data set.

protocol SupervisedTemporalEstimator

An estimator that creates a transformer by fitting to a sequence of annotated temporal features.

Deprecated

protocol UpdatableEstimator

An estimator that can be incrementally updated.

protocol UpdatableSupervisedEstimator

A supervised estimator that can be incrementally updated.

protocol UpdatableSupervisedTemporalEstimator

A supervised temporal estimator that can be incrementally updated.

Deprecated

protocol UpdatableSupervisedTabularEstimator

A supervised tabular estimator that can be incrementally updated.

protocol UpdatableTemporalEstimator

A temporal estimator that can be incrementally updated.

Deprecated

protocol UpdatableTabularEstimator

A tabular estimator that can be incrementally updated.

