

- Create ML Components
-  TemporalTransformerToEstimatorAdaptor Deprecated

Structure

# TemporalTransformerToEstimatorAdaptor

A temporal estimator that always returns a predefined temporal transformer.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
struct TemporalTransformerToEstimatorAdaptor where Transformer : TemporalTransformer
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

### Fitting

func fitted&lt;InputSequence>(to: InputSequence, eventHandler: EventHandler?) async throws -> Transformer

Returns the pre-defined transformer.

### Default Implementations

TemporalEstimator Implementations

## Relationships

### Conforms To

- Sendable
- TemporalEstimator

## See Also

### Temporal adaptors

struct TemporalAdaptor

A temporal transformer that applies a regular transformer to each value of a temporal sequence.

struct TemporalEstimatorToSupervisedAdaptor

An adaptor that exposes a temporal estimator as a supervised temporal estimator.

Deprecated

struct TemporalTransformerToUpdatableEstimatorAdaptor

A temporal estimator that always returns a predefined temporal transformer.

Deprecated

