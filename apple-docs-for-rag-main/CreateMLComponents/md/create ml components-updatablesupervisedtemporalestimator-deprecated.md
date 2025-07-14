

- Create ML Components
-  UpdatableSupervisedTemporalEstimator Deprecated

Protocol

# UpdatableSupervisedTemporalEstimator

A supervised temporal estimator that can be incrementally updated.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
protocol UpdatableSupervisedTemporalEstimator : SupervisedTemporalEstimator
```

## Topics

### Appending

func appending&lt;Other>(Other) -> some UpdatableSupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;Self.Transformer, Other.Transformer>, Self.Annotation> 

Composes this updatable supervised temporal estimator with another updatable supervised temporal estimator.

func appending&lt;Other>(Other) -> some UpdatableSupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;Self.Transformer, Other.Transformer>, Self.Annotation> 

Composes this updatable supervised temporal estimator with an updatable temporal estimator.

func appending&lt;Other>(Other) -> some UpdatableSupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;Self.Transformer, TransformerToTemporalAdaptor&lt;Other>>, Self.Annotation> 

Composes this updatable supervised temporal estimator with a transformer.

func appending&lt;Other>(Other) -> some UpdatableSupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;Self.Transformer, TransformerToTemporalAdaptor&lt;Other.Transformer>>, Self.Annotation> 

Composes this updatable supervised temporal estimator with an updatable estimator.

func appending&lt;Other>(Other) -> some UpdatableSupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;Self.Transformer, TransformerToTemporalAdaptor&lt;Other.Transformer>>, Self.Annotation> 

Composes this updatable supervised temporal estimator with an updatable supervised estimator.

func appending&lt;Other>(Other) -> some UpdatableSupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;Self.Transformer, Other>, Self.Annotation> 

Composes this updatable supervised temporal estimator with a transformer.

### Encoding and decoding

func encodeWithOptimizer(Self.Transformer, to: inout any EstimatorEncoder) throws

Encodes the transformer and optimizer to an encoder.

**Required**

func decodeWithOptimizer(from: inout any EstimatorDecoder) throws -> Self.Transformer

Reads the encoded transformer and optimizer with a decoder.

**Required**

### Reading and writing

func readWithOptimizer(from: URL) throws -> Self.Transformer

Reads the encoded transformer and optimizer from a file.

func writeWithOptimizer(Self.Transformer, to: URL, overwrite: Bool) throws

Writes the encoded transformer and optimizer to a file.

### Transforming

func makeTransformer() -> Self.Transformer

Creates a default-initialized transformer suitable for incremental fitting.

**Required**

func update&lt;InputSequence, FeatureSequence>(inout Self.Transformer, with: InputSequence, eventHandler: EventHandler?) async throws

Updates a transformer with a new sequence of examples.

**Required**

func update&lt;InputSequence, FeatureSequence>(inout Self.Transformer, with: InputSequence) async throws

## Relationships

### Inherits From

- SupervisedTemporalEstimator

### Conforming Types

- PreprocessingUpdatableSupervisedTemporalEstimator
- UpdatableSupervisedEstimatorToTemporalAdaptor
- UpdatableTemporalEstimatorToSupervisedAdaptor

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

protocol UpdatableSupervisedTabularEstimator

A supervised tabular estimator that can be incrementally updated.

protocol UpdatableTemporalEstimator

A temporal estimator that can be incrementally updated.

Deprecated

protocol UpdatableTabularEstimator

A tabular estimator that can be incrementally updated.

