

- Create ML Components
-  UpdatableTabularEstimator 

Protocol

# UpdatableTabularEstimator

A tabular estimator that can be incrementally updated.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
protocol UpdatableTabularEstimator : TabularEstimator
```

## Topics

### Appending

func appending&lt;Other>(Other) -> some UpdatableTabularEstimator&lt;ComposedTabularTransformer&lt;Self.Transformer, Other>> 

Composes this updatable tabular estimator with a tabular transformer.

func appending&lt;Other>(Other) -> some UpdatableTabularEstimator&lt;ComposedTabularTransformer&lt;Self.Transformer, Other.Transformer>> 

Composes this updatable tabular estimator with another updatable tabular estimator.

func appending&lt;Other>(Other) -> some UpdatableSupervisedTabularEstimator&lt;ComposedTabularTransformer&lt;Self.Transformer, Other.Transformer>, Other.Annotation> 

Composes this updatable tabular estimator with an updatable supervised tabular estimator.

### Adapting

func adaptedAsSupervised&lt;Annotation>(annotationColumnID: ColumnID&lt;Annotation>) -> UpdatableTabularEstimatorToSupervisedAdaptor&lt;Self, Annotation>

Exposes this updatable tabular estimator as a supervised tabular estimator.

### Encoding and decoding

func encodeWithOptimizer(Self.Transformer, to: inout any EstimatorEncoder) throws

Encodes the transformer and optimizer to an encoder.

**Required**

func decodeWithOptimizer(from: inout any EstimatorDecoder) throws -> Self.Transformer

Reads the encoded transformer and optimizer with a decoder.

**Required**

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

- TabularEstimator

### Conforming Types

- ColumnSelector

  Conforms when `Estimator` conforms to `UpdatableEstimator`, `UnwrappedInput` conforms to `Copyable`, `UnwrappedInput` conforms to `Escapable`, and `Estimator.Transformer.Input` is `UnwrappedInput?`.

- PreprocessingUpdatableTabularEstimator
- TabularTransformerToUpdatableEstimatorAdaptor

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

protocol UpdatableSupervisedTabularEstimator

A supervised tabular estimator that can be incrementally updated.

protocol UpdatableTemporalEstimator

A temporal estimator that can be incrementally updated.

Deprecated

