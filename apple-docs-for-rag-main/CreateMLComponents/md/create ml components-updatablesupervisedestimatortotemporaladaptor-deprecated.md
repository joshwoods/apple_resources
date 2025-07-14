

- Create ML Components
-  UpdatableSupervisedEstimatorToTemporalAdaptor Deprecated

Structure

# UpdatableSupervisedEstimatorToTemporalAdaptor

An updatable supervised temporal estimator wrapping an updatable supervised estimator.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
struct UpdatableSupervisedEstimatorToTemporalAdaptor where Base : UpdatableSupervisedEstimator, Base.Annotation : Sendable
```

## Topics

### Creating an adaptor

init(Base)

Creates a temporal supervised estimator from a supervised estimator.

### Encoding and decoding

func encode(UpdatableSupervisedEstimatorToTemporalAdaptor&lt;Base>.Transformer, to: inout any EstimatorEncoder) throws

Encodes a fitted transformer.

func decode(from: inout any EstimatorDecoder) throws -> UpdatableSupervisedEstimatorToTemporalAdaptor&lt;Base>.Transformer

Decodes the transformer.

func encodeWithOptimizer(UpdatableSupervisedEstimatorToTemporalAdaptor&lt;Base>.Transformer, to: inout any EstimatorEncoder) throws

Encodes the transformer and optimizer to an encoder.

func decodeWithOptimizer(from: inout any EstimatorDecoder) throws -> UpdatableSupervisedEstimatorToTemporalAdaptor&lt;Base>.Transformer

Reads the encoded transformer and optimizer with a decoder.

### Fitting and updating

func fitted&lt;InputSequence, FeatureSequence>(to: InputSequence, eventHandler: EventHandler?) async throws -> UpdatableSupervisedEstimatorToTemporalAdaptor&lt;Base>.Transformer

Fits a transformer to a sequence of examples.

func fitted&lt;InputSequence, Validation, FeatureSequence>(to: InputSequence, validateOn: Validation, eventHandler: EventHandler?) async throws -> UpdatableSupervisedEstimatorToTemporalAdaptor&lt;Base>.Transformer

Fits a transformer to a sequence of examples while validating with a validation sequence.

func makeTransformer() -> UpdatableSupervisedEstimatorToTemporalAdaptor&lt;Base>.Transformer

Creates a default-initialized transformer suitable for incremental fitting.

func update&lt;InputSequence, FeatureSequence>(inout UpdatableSupervisedEstimatorToTemporalAdaptor&lt;Base>.Transformer, with: InputSequence, eventHandler: EventHandler?) async throws

Updates a transformer with a new sequence of examples.

typealias Annotation

The annotation type.

typealias Input

The input type.

typealias Output

The output type.

typealias Transformer

The transformer type created by this estimator.

### Default Implementations

SupervisedTemporalEstimator Implementations

UpdatableSupervisedTemporalEstimator Implementations

## Relationships

### Conforms To

- Sendable
- SupervisedTemporalEstimator
- UpdatableSupervisedTemporalEstimator

## See Also

### Updatable adaptors

struct UpdatableEstimatorToTemporalAdaptor

An updatable temporal estimator wrapping an updatable estimator.

Deprecated

struct UpdatableEstimatorToSupervisedAdaptor

An adaptor that exposes an updatable estimator as an updatable supervised estimator.

struct UpdatableTemporalEstimatorToSupervisedAdaptor

An adaptor that exposes an updatable temporal estimator as an updatable supervised temporal estimator.

Deprecated

