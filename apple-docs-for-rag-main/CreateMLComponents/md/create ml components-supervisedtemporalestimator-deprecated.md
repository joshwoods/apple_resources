

- Create ML Components
-  SupervisedTemporalEstimator Deprecated

Protocol

# SupervisedTemporalEstimator

An estimator that creates a transformer by fitting to a sequence of annotated temporal features.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
protocol SupervisedTemporalEstimator
```

## Topics

### Reading and writing

func read(from: URL) throws -> Self.Transformer

Reads the encoded transformer from a file.

func write(Self.Transformer, to: URL, overwrite: Bool) throws

Writes the encoded transformer to a file.

associatedtype Annotation : Equatable, Sendable

The annotation type.

**Required**

associatedtype Transformer : TemporalTransformer

The transformer type created by this estimator.

**Required**

### Appending

func appending&lt;Other>(Other) -> some SupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;Self.Transformer, TransformerToTemporalAdaptor&lt;Other.Transformer>>, Self.Annotation> 

Composes this supervised temporal estimator with a supervised estimator.

func appending&lt;Other>(Other) -> some SupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;Self.Transformer, Other>, Self.Annotation> 

Composes this supervised temporal estimator with a transformer.

func appending&lt;Other>(Other) -> some SupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;Self.Transformer, Other.Transformer>, Self.Annotation> 

Composes this supervised temporal estimator with another supervised temporal estimator.

func appending&lt;Other>(Other) -> some SupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;Self.Transformer, Other.Transformer>, Self.Annotation> 

Composes this supervised temporal estimator with a temporal estimator.

func appending&lt;Other>(Other) -> some SupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;Self.Transformer, TransformerToTemporalAdaptor&lt;Other.Transformer>>, Self.Annotation> 

Composes this supervised temporal estimator with an estimator.

func appending&lt;Other>(Other) -> some SupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;Self.Transformer, TransformerToTemporalAdaptor&lt;Other>>, Self.Annotation> 

Composes this supervised temporal estimator with a transformer.

### Fitting

func fitted&lt;InputSequence, FeatureSequence>(to: InputSequence) async throws -> Self.Transformer

func fitted&lt;InputSequence, FeatureSequence>(to: InputSequence, eventHandler: EventHandler?) async throws -> Self.Transformer

Fits a transformer to a sequence of examples.

**Required**

func fitted&lt;InputSequence, Validation, FeatureSequence>(to: InputSequence, validateOn: Validation) async throws -> Self.Transformer

func fitted&lt;InputSequence, Validation, FeatureSequence>(to: InputSequence, validateOn: Validation, eventHandler: EventHandler?) async throws -> Self.Transformer

Fits a transformer to a sequence of examples while validating with a validation sequence.

**Required**

associatedtype Annotation : Equatable, Sendable

The annotation type.

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

- UpdatableSupervisedTemporalEstimator

### Conforming Types

- PreprocessingSupervisedTemporalEstimator
- PreprocessingUpdatableSupervisedTemporalEstimator
- SupervisedEstimatorToTemporalAdaptor
- TemporalEstimatorToSupervisedAdaptor
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

