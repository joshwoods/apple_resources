

- Create ML Components
-  TemporalEstimator Deprecated

Protocol

# TemporalEstimator

An estimator that creates a transformer by fitting to a sequence of temporal features.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
protocol TemporalEstimator
```

## Topics

### Reading and writing

func read(from: URL) throws -> Self.Transformer

Reads the encoded transformer from a file.

func write(Self.Transformer, to: URL, overwrite: Bool) throws

Writes the encoded transformer to a file.

### Appending

func appending&lt;Other>(Other) -> some TemporalEstimator&lt;ComposedTemporalTransformer&lt;Self.Transformer, Other>> 

Composes this temporal estimator with a temporal transformer.

func appending&lt;Other>(Other) -> some SupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;Self.Transformer, Other.Transformer>, Other.Annotation> 

Composes this temporal estimator with a supervised temporal estimator.

func appending&lt;Other>(Other) -> some TemporalEstimator&lt;ComposedTemporalTransformer&lt;Self.Transformer, TransformerToTemporalAdaptor&lt;Other.Transformer>>> 

Composes this temporal estimator with an estimator.

func appending&lt;Other>(Other) -> some TemporalEstimator&lt;ComposedTemporalTransformer&lt;Self.Transformer, TransformerToTemporalAdaptor&lt;Other>>> 

Composes this temporal estimator with a transformer.

func appending&lt;Other>(Other) -> some SupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;Self.Transformer, TransformerToTemporalAdaptor&lt;Other.Transformer>>, Other.Annotation> 

Composes this temporal estimator with a supervised temporal estimator.

func appending&lt;Other>(Other) -> some TemporalEstimator&lt;ComposedTemporalTransformer&lt;Self.Transformer, Other.Transformer>> 

Composes this temporal estimator with another temporal estimator.

### Adapting and fitting

func adaptedAsSupervised&lt;Annotation>(annotationType: Annotation.Type) -> TemporalEstimatorToSupervisedAdaptor&lt;Self, Annotation>

Exposes this temporal estimator as a supervised temporal estimator.

func fitted&lt;InputSequence>(to: InputSequence) async throws -> Self.Transformer

func fitted&lt;InputSequence>(to: InputSequence, eventHandler: EventHandler?) async throws -> Self.Transformer

Fits a transformer to a sequence of examples.

**Required**

associatedtype Transformer : TemporalTransformer

The transformer type created by this estimator.

**Required**

### Encoding and decoding

func encode(Self.Transformer, to: inout any EstimatorEncoder) throws

Encodes a fitted transformer.

**Required**

func decode(from: inout any EstimatorDecoder) throws -> Self.Transformer

Decodes a previously fitted transformer.

**Required**

## Relationships

### Inherited By

- UpdatableTemporalEstimator

### Conforming Types

- EstimatorToTemporalAdaptor
- PreprocessingTemporalEstimator
- PreprocessingUpdatableTemporalEstimator
- TemporalTransformerToEstimatorAdaptor
- TemporalTransformerToUpdatableEstimatorAdaptor
- UpdatableEstimatorToTemporalAdaptor

## See Also

### Protocols

protocol Transformer

A transformer that takes an input and produces an output.

protocol TemporalTransformer

A transformer that takes an asynchronous input sequence of temporal features and produces an asynchronous output sequence.

protocol RandomTransformer

A transformer that takes an input and a random number generator and produces a randomized output.

protocol Estimator

An estimator that creates a transformer by fitting to a data set.

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

