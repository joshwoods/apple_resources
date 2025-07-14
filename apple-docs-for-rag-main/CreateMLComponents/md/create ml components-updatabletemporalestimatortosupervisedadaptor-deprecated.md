

- Create ML Components
-  UpdatableTemporalEstimatorToSupervisedAdaptor Deprecated

Structure

# UpdatableTemporalEstimatorToSupervisedAdaptor

An adaptor that exposes an updatable temporal estimator as an updatable supervised temporal estimator.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
struct UpdatableTemporalEstimatorToSupervisedAdaptor where Estimator : UpdatableTemporalEstimator, Annotation : Equatable, Annotation : Sendable
```

## Topics

### Creating an adaptor

init(Estimator)

Creates a temporal estimator adaptor.

### Getting the estimator

let estimator: Estimator

The wrapped estimator.

### Encoding and decoding

func encode(UpdatableTemporalEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer, to: inout any EstimatorEncoder) throws

Does nothing since this estimator uses a pre-defined transformer.

func decode(from: inout any EstimatorDecoder) throws -> UpdatableTemporalEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer

Returns the pre-defined transformer.

func encodeWithOptimizer(UpdatableTemporalEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer, to: inout any EstimatorEncoder) throws

Encodes the transformer and optimizer to an encoder.

func decodeWithOptimizer(from: inout any EstimatorDecoder) throws -> UpdatableTemporalEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer

Reads the encoded transformer and optimizer with a decoder.

### Fitting and updating

func fitted&lt;InputSequence, FeatureSequence>(to: InputSequence, eventHandler: EventHandler?) async throws -> UpdatableTemporalEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer

Fits a transformer to a sequence of examples.

func fitted&lt;InputSequence, Validation, FeatureSequence>(to: InputSequence, validateOn: Validation, eventHandler: EventHandler?) async throws -> UpdatableTemporalEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer

Fits a transformer to a sequence of examples while validating with a validation sequence.

func makeTransformer() -> Estimator.Transformer

Creates a default-initialized transformer suitable for incremental fitting.

func update&lt;InputSequence, FeatureSequence>(inout UpdatableTemporalEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer, with: InputSequence, eventHandler: EventHandler?) async throws

Updates a transformer with a new sequence of examples.

func update&lt;InputSequence, Validation, FeatureSequence>(inout UpdatableTemporalEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer, with: InputSequence, validateOn: Validation, eventHandler: EventHandler?) async throws

Fits a transformer to a sequence of examples while validating with a validation sequence.

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

struct UpdatableSupervisedEstimatorToTemporalAdaptor

An updatable supervised temporal estimator wrapping an updatable supervised estimator.

Deprecated

