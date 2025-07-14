

- Create ML Components
-  TemporalTransformerToUpdatableEstimatorAdaptor Deprecated

Structure

# TemporalTransformerToUpdatableEstimatorAdaptor

A temporal estimator that always returns a predefined temporal transformer.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
struct TemporalTransformerToUpdatableEstimatorAdaptor where Transformer : TemporalTransformer
```

## Topics

### Creating an estimator

init(Transformer)

Creates a trivial estimator.

### Getting the transformer

let transformer: Transformer

A pre-defined transformer.

### Encoding and decoding

func encode(Transformer, to: inout any EstimatorEncoder) throws

Does nothing since this estimator uses a pre-defined transformer.

func decode(from: inout any EstimatorDecoder) throws -> Transformer

Returns the pre-defined transformer.

func encodeWithOptimizer(Transformer, to: inout any EstimatorEncoder) throws

This method is part of the conformance. It doesn’t encode anything since the transformer is pre-defined, so don’t call it.

func decodeWithOptimizer(from: inout any EstimatorDecoder) throws -> Transformer

Returns the pre-defined transformer.

### Fitting and updating

func fitted&lt;InputSequence>(to: InputSequence, eventHandler: EventHandler?) async throws -> Transformer

Returns the pre-defined transformer.

func makeTransformer() -> Transformer

Creates a default-initialized transformer suitable for incremental fitting.

func update&lt;InputSequence>(inout Transformer, with: InputSequence, eventHandler: EventHandler?) async throws

Does nothing since this estimator uses a pre-defined transformer.

### Default Implementations

TemporalEstimator Implementations

UpdatableTemporalEstimator Implementations

## Relationships

### Conforms To

- Sendable
- TemporalEstimator
- UpdatableTemporalEstimator

## See Also

### Temporal adaptors

struct TemporalAdaptor

A temporal transformer that applies a regular transformer to each value of a temporal sequence.

struct TemporalTransformerToEstimatorAdaptor

A temporal estimator that always returns a predefined temporal transformer.

Deprecated

struct TemporalEstimatorToSupervisedAdaptor

An adaptor that exposes a temporal estimator as a supervised temporal estimator.

Deprecated

