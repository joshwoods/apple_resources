

- Create ML Components
-  UpdatableEstimatorToTemporalAdaptor Deprecated

Structure

# UpdatableEstimatorToTemporalAdaptor

An updatable temporal estimator wrapping an updatable estimator.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
struct UpdatableEstimatorToTemporalAdaptor where Base : UpdatableEstimator
```

## Topics

### Creating an adaptor

init(Base)

Creates a temporal estimator from an estimator.

### Encoding and decoding

func encode(UpdatableEstimatorToTemporalAdaptor&lt;Base>.Transformer, to: inout any EstimatorEncoder) throws

Encodes a fitted transformer.

func decode(from: inout any EstimatorDecoder) throws -> UpdatableEstimatorToTemporalAdaptor&lt;Base>.Transformer

Decodes the transformer.

func encodeWithOptimizer(UpdatableEstimatorToTemporalAdaptor&lt;Base>.Transformer, to: inout any EstimatorEncoder) throws

Encodes the transformer and optimizer to an encoder.

func decodeWithOptimizer(from: inout any EstimatorDecoder) throws -> UpdatableEstimatorToTemporalAdaptor&lt;Base>.Transformer

Reads the encoded transformer and optimizer with a decoder.

### Fitting and updating

func fitted&lt;InputSequence>(to: InputSequence, eventHandler: EventHandler?) async throws -> UpdatableEstimatorToTemporalAdaptor&lt;Base>.Transformer

Fits a transformer to a sequence of examples.

func makeTransformer() -> UpdatableEstimatorToTemporalAdaptor&lt;Base>.Transformer

Creates a default-initialized transformer suitable for incremental fitting.

func update&lt;InputSequence>(inout UpdatableEstimatorToTemporalAdaptor&lt;Base>.Transformer, with: InputSequence, eventHandler: EventHandler?) async throws

Updates a transformer with a new sequence of examples.

typealias Input

The input type.

typealias Output

The output type.

typealias Transformer

The transformer type created by this estimator.

### Default Implementations

TemporalEstimator Implementations

UpdatableTemporalEstimator Implementations

## Relationships

### Conforms To

- Sendable
- TemporalEstimator
- UpdatableTemporalEstimator

## See Also

### Updatable adaptors

struct UpdatableEstimatorToSupervisedAdaptor

An adaptor that exposes an updatable estimator as an updatable supervised estimator.

struct UpdatableSupervisedEstimatorToTemporalAdaptor

An updatable supervised temporal estimator wrapping an updatable supervised estimator.

Deprecated

struct UpdatableTemporalEstimatorToSupervisedAdaptor

An adaptor that exposes an updatable temporal estimator as an updatable supervised temporal estimator.

Deprecated

