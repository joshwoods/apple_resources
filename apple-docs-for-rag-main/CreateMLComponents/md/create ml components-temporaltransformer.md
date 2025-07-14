

- Create ML Components
-  TemporalTransformer 

Protocol

# TemporalTransformer

A transformer that takes an asynchronous input sequence of temporal features and produces an asynchronous output sequence.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
protocol TemporalTransformer
```

## Overview

A temporal transformer, unlike a regular transformer, can accumulate multiple inputs before producing an output. For example, an audio transformer can accumulate audio buffers until the desired length is reached before producing an output.

## Topics

### Applying and adapting

func applied&lt;S>(to: S, eventHandler: EventHandler?) async throws -> Self.OutputSequence

Performs the transformation on an input sequence.

**Required** Default implementations provided.

func adaptedAsEstimator() -> TemporalTransformerToEstimatorAdaptor&lt;Self>

Exposes this temporal transformer as a trivial temporal estimator.

Deprecated

func adaptedAsUpdatableEstimator() -> TemporalTransformerToUpdatableEstimatorAdaptor&lt;Self>

Exposes this temporal transformer as a trivial temporal estimator.

Deprecated

associatedtype Input

The input type.

**Required**

associatedtype Output

The output type.

**Required**

associatedtype OutputSequence : TemporalSequence

The output async sequence type.

**Required**

### Appending

func appending&lt;Other>(Other) -> ComposedTemporalTransformer&lt;Self, TransformerToTemporalAdaptor&lt;Other>>

Composes this temporal transformer with a transformer.

Deprecated

func appending&lt;Other>(Other) -> ComposedTemporalTransformer&lt;Self, Other>

Composes this temporal transformer with another temporal transformer.

func appending&lt;Other>(Other) -> PreprocessingSupervisedTemporalEstimator&lt;Self, Other>

Composes this transformer with a supervised temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> PreprocessingUpdatableTemporalEstimator&lt;Self, Other>

Composes this temporal transformer with an updatable temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> PreprocessingUpdatableSupervisedTemporalEstimator&lt;Self, UpdatableSupervisedEstimatorToTemporalAdaptor&lt;Other>>

Composes this transformer with an updatable supervised temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> PreprocessingTemporalEstimator&lt;Self, Other>

Composes this temporal transformer with a temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> PreprocessingTemporalEstimator&lt;Self, EstimatorToTemporalAdaptor&lt;Other>>

Composes this temporal transformer with an estimator.

Deprecated

func appending&lt;Other>(Other) -> PreprocessingUpdatableTemporalEstimator&lt;Self, UpdatableEstimatorToTemporalAdaptor&lt;Other>>

Composes this temporal transformer with an updatable estimator.

Deprecated

func appending&lt;Other>(Other) -> PreprocessingSupervisedTemporalEstimator&lt;Self, SupervisedEstimatorToTemporalAdaptor&lt;Other>>

Composes this transformer with a supervised temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> PreprocessingUpdatableSupervisedTemporalEstimator&lt;Self, Other>

Composes this transformer with an updatable supervised temporal estimator.

Deprecated

### Transforming and predicting

func callAsFunction&lt;S>(S, eventHandler: EventHandler?) async throws -> Self.OutputSequence

Performs the transformation on an input sequence.

func callAsFunction&lt;S>(to: S, eventHandler: EventHandler?) async throws -> [Self.OutputSequence]

Performs the transformation on a sequence of inputs.

func prediction&lt;S, Label>(from: S) async throws -> Self.OutputSequence

Performs a prediction on a single input.

### Exporting

func export(to: URL) throws

Exports this temporal transformer as a CoreML model.

func export(to: URL, metadata: ModelMetadata) throws

Exports this temporal transformer as a CoreML model with user-supplied metadata.

### Instance Methods

func appending&lt;Other>(Other) -> ComposedTemporalTransformer&lt;Self, TemporalAdaptor&lt;Other>>

Composes this temporal transformer with a transformer.

## Relationships

### Conforming Types

- AudioFeaturePrint
- ComposedTemporalTransformer
- Downsampler
- HumanBodyActionCounter
- LinearTimeSeriesForecaster.Model

  Conforms when `Scalar` conforms to `MLShapedArrayScalar` and `BinaryFloatingPoint`.

- SlidingWindowTransformer
- TemporalAdaptor
- TimeSeriesClassifier.Model

  Conforms when `Scalar` conforms to `MLShapedArrayScalar`, `Scalar` conforms to `BinaryFloatingPoint`, `Label` conforms to `Comparable`, `Label` conforms to `Decodable`, `Label` conforms to `Encodable`, and `Label` conforms to `Hashable`.

- TransformerToTemporalAdaptor

## See Also

### Protocols

protocol Transformer

A transformer that takes an input and produces an output.

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

protocol UpdatableTabularEstimator

A tabular estimator that can be incrementally updated.

