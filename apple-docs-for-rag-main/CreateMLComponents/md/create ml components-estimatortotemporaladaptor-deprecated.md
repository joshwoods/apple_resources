

- Create ML Components
-  EstimatorToTemporalAdaptor Deprecated

Structure

# EstimatorToTemporalAdaptor

A temporal estimator wrapping an estimator.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
struct EstimatorToTemporalAdaptor where Base : Estimator
```

## Topics

### Creating the estimator

init(Base)

Creates a temporal estimator from an estimator.

### Encoding and decoding

func encode(EstimatorToTemporalAdaptor&lt;Base>.Transformer, to: inout any EstimatorEncoder) throws

Encodes a fitted transformer.

func decode(from: inout any EstimatorDecoder) throws -> EstimatorToTemporalAdaptor&lt;Base>.Transformer

Decodes the transformer.

### Fitting a transformer

func fitted&lt;InputSequence>(to: InputSequence, eventHandler: EventHandler?) async throws -> EstimatorToTemporalAdaptor&lt;Base>.Transformer

Fits a transformer to a sequence of examples.

typealias Input

The input type.

typealias Output

The output type.

typealias Transformer

The transformer type created by this estimator.

### Default Implementations

TemporalEstimator Implementations

## Relationships

### Conforms To

- Sendable
- TemporalEstimator

## See Also

### Estimator adaptors

struct EstimatorToSupervisedAdaptor

An adaptor that exposes an estimator as a supervised estimator.

struct SupervisedEstimatorToTemporalAdaptor

A supervised temporal estimator wrapping a supervised estimator.

Deprecated

