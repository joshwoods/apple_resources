

- Create ML Components
-  UpdatableSupervisedEstimator 

Protocol

# UpdatableSupervisedEstimator

A supervised estimator that can be incrementally updated.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
protocol UpdatableSupervisedEstimator : SupervisedEstimator
```

## Topics

### Appending

func appending&lt;Other>(Other) -> some UpdatableSupervisedEstimator&lt;ComposedTransformer&lt;Self.Transformer, Other.Transformer>, Self.Annotation> 

Composes this updatable estimator with an updatable estimator.

func appending&lt;Other>(Other) -> some UpdatableSupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;TransformerToTemporalAdaptor&lt;Self.Transformer>, Other.Transformer>, Self.Annotation> 

Composes this updatable supervised estimator with an updatable temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> some UpdatableSupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;TransformerToTemporalAdaptor&lt;Self.Transformer>, Other>, Self.Annotation> 

Composes this updatable supervised estimator with a temporal transformer.

Deprecated

func appending&lt;Other>(Other) -> some UpdatableSupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;TransformerToTemporalAdaptor&lt;Self.Transformer>, Other.Transformer>, Self.Annotation> 

Composes this updatable supervised estimator with an updatable supervised temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> some UpdatableSupervisedEstimator&lt;ComposedTransformer&lt;Self.Transformer, Other>, Self.Annotation> 

Composes this updatable estimator with a transformer.

func appending&lt;Other>(Other) -> some UpdatableSupervisedEstimator&lt;ComposedTransformer&lt;Self.Transformer, Other.Transformer>, Self.Annotation> 

Composes this updatable estimator with an updatable supervised estimator.

### Adapting

func adaptedAsTemporal() -> UpdatableSupervisedEstimatorToTemporalAdaptor&lt;Self>

Exposes this supervised estimator as a temporal supervised estimator.

Deprecated

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

func update&lt;InputSequence>(inout Self.Transformer, with: InputSequence, eventHandler: EventHandler?) async throws

Updates a transformer with a new sequence of examples.

**Required** Default implementation provided.

func update&lt;InputSequence>(inout Self.Transformer, with: InputSequence) async throws

## Relationships

### Inherits From

- SupervisedEstimator

### Conforming Types

- FullyConnectedNetworkClassifier

  Conforms when `Scalar` conforms to `MLShapedArrayScalar`, `Scalar` conforms to `BinaryFloatingPoint`, `Label` conforms to `Comparable`, `Label` conforms to `Decodable`, `Label` conforms to `Encodable`, and `Label` conforms to `Hashable`.

- FullyConnectedNetworkMultiLabelClassifier

  Conforms when `Scalar` conforms to `MLShapedArrayScalar`, `Scalar` conforms to `BinaryFloatingPoint`, `Scalar` conforms to `Decodable`, `Scalar` conforms to `Encodable`, `Label` conforms to `Comparable`, `Label` conforms to `Decodable`, `Label` conforms to `Encodable`, and `Label` conforms to `Hashable`.

- FullyConnectedNetworkRegressor

  Conforms when `Scalar` conforms to `MLShapedArrayScalar` and `BinaryFloatingPoint`.

- LinearRegressor

  Conforms when `Scalar` conforms to `MLShapedArrayScalar` and `BinaryFloatingPoint`.

- LinearTimeSeriesForecaster

  Conforms when `Scalar` conforms to `MLShapedArrayScalar` and `BinaryFloatingPoint`.

- LogisticRegressionClassifier

  Conforms when `Scalar` conforms to `MLShapedArrayScalar`, `Scalar` conforms to `BinaryFloatingPoint`, `Label` conforms to `Comparable`, `Label` conforms to `Decodable`, `Label` conforms to `Encodable`, and `Label` conforms to `Hashable`.

- MultivariateLinearRegressor

  Conforms when `Scalar` conforms to `MLShapedArrayScalar` and `BinaryFloatingPoint`.

- PreprocessingUpdatableSupervisedEstimator
- TimeSeriesClassifier

  Conforms when `Scalar` conforms to `MLShapedArrayScalar`, `Scalar` conforms to `BinaryFloatingPoint`, `Label` conforms to `Comparable`, `Label` conforms to `Decodable`, `Label` conforms to `Encodable`, and `Label` conforms to `Hashable`.

- UpdatableEstimatorToSupervisedAdaptor

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

