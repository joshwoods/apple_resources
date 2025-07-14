

- Create ML Components
-  UpdatableEstimatorToSupervisedAdaptor 

Structure

# UpdatableEstimatorToSupervisedAdaptor

An adaptor that exposes an updatable estimator as an updatable supervised estimator.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct UpdatableEstimatorToSupervisedAdaptor where Estimator : UpdatableEstimator, Annotation : Equatable
```

## Topics

### Creating an adaptor

init(Estimator)

Creates an estimator adaptor.

### Getting the estimator

let estimator: Estimator

The wrapped estimator.

### Encoding and decoding

func encode(UpdatableEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer, to: inout any EstimatorEncoder) throws

Does nothing since this estimator uses a pre-defined transformer.

func decode(from: inout any EstimatorDecoder) throws -> UpdatableEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer

Returns the pre-defined transformer.

func encodeWithOptimizer(UpdatableEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer, to: inout any EstimatorEncoder) throws

Encodes the transformer and optimizer to an encoder.

func decodeWithOptimizer(from: inout any EstimatorDecoder) throws -> UpdatableEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer

Reads the encoded transformer and optimizer.

### Fitting and Updating

func fitted&lt;Input>(to: Input, eventHandler: EventHandler?) async throws -> UpdatableEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer

Fits a transformer to a sequence of examples, ignoring the annotations and the validation.

func fitted&lt;Input, Validation>(to: Input, validateOn: Validation, eventHandler: EventHandler?) async throws -> UpdatableEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer

Fits a transformer to a sequence of examples.

func makeTransformer() -> Estimator.Transformer

Creates a default-initialized transformer suitable for incremental fitting.

func update&lt;InputSequence>(inout Estimator.Transformer, with: InputSequence, eventHandler: EventHandler?) async throws

Updates a transformer with a new sequence of examples.

func update&lt;InputSequence, Validation>(inout Estimator.Transformer, with: InputSequence, validateOn: Validation, eventHandler: EventHandler?) async throws

Fits a transformer to a sequence of examples while validating with a validation sequence.

typealias Transformer

The transformer type created by this estimator.

### Default Implementations

SupervisedEstimator Implementations

UpdatableSupervisedEstimator Implementations

## Relationships

### Conforms To

- Sendable
- SupervisedEstimator
- UpdatableSupervisedEstimator

## See Also

### Updatable adaptors

struct UpdatableEstimatorToTemporalAdaptor

An updatable temporal estimator wrapping an updatable estimator.

Deprecated

struct UpdatableSupervisedEstimatorToTemporalAdaptor

An updatable supervised temporal estimator wrapping an updatable supervised estimator.

Deprecated

struct UpdatableTemporalEstimatorToSupervisedAdaptor

An adaptor that exposes an updatable temporal estimator as an updatable supervised temporal estimator.

Deprecated

