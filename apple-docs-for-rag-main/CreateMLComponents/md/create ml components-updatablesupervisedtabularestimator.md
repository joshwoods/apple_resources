

- Create ML Components
-  UpdatableSupervisedTabularEstimator 

Protocol

# UpdatableSupervisedTabularEstimator

A supervised tabular estimator that can be incrementally updated.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
protocol UpdatableSupervisedTabularEstimator : SupervisedTabularEstimator
```

## Topics

### Appending

func appending&lt;Other>(Other) -> some UpdatableSupervisedTabularEstimator&lt;ComposedTabularTransformer&lt;Self.Transformer, Other.Transformer>, Self.Annotation> 

Composes this supervised tabular estimator with another supervised tabular estimator.

func appending&lt;Other>(Other) -> some UpdatableSupervisedTabularEstimator&lt;ComposedTabularTransformer&lt;Self.Transformer, Other.Transformer>, Self.Annotation> 

Composes this supervised tabular estimator with an updatable tabular estimator.

func appending&lt;Other>(Other) -> some UpdatableSupervisedTabularEstimator&lt;ComposedTabularTransformer&lt;Self.Transformer, Other>, Self.Annotation> 

Composes this supervised tabular estimator with a tabular transformer.

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

func update(inout Self.Transformer, with: DataFrame) async throws

func update(inout Self.Transformer, with: DataFrame, eventHandler: EventHandler?) async throws

Updates a transformer with a new sequence of examples.

**Required**

## Relationships

### Inherits From

- SupervisedTabularEstimator

### Conforming Types

- AnnotatedFeatureProvider

  Conforms when `Base` conforms to `UpdatableSupervisedEstimator`, `UnwrappedInput` conforms to `Copyable`, `UnwrappedInput` conforms to `Escapable`, and `Base.Transformer.Input` is `UnwrappedInput?`.

- BoostedTreeClassifier

  Conforms when `Label` conforms to `Comparable`, `Decodable`, `Encodable`, and `Hashable`.

- BoostedTreeRegressor

  Conforms when `Annotation` conforms to `Copyable` and `Escapable`.

- PreprocessingUpdatableSupervisedTabularEstimator
- UpdatableTabularEstimatorToSupervisedAdaptor

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

protocol UpdatableSupervisedTemporalEstimator

A supervised temporal estimator that can be incrementally updated.

Deprecated

protocol UpdatableTemporalEstimator

A temporal estimator that can be incrementally updated.

Deprecated

protocol UpdatableTabularEstimator

A tabular estimator that can be incrementally updated.

