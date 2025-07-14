

- Create ML Components
-  SupervisedEstimatorToTemporalAdaptor Deprecated

Structure

# SupervisedEstimatorToTemporalAdaptor

A supervised temporal estimator wrapping a supervised estimator.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
struct SupervisedEstimatorToTemporalAdaptor where Base : SupervisedEstimator, Base.Annotation : Sendable
```

## Topics

### Creating an estimator

init(Base)

Creates a temporal supervised estimator from a supervised estimator.

### Encoding and decoding

func encode(SupervisedEstimatorToTemporalAdaptor&lt;Base>.Transformer, to: inout any EstimatorEncoder) throws

Encodes a fitted transformer.

func decode(from: inout any EstimatorDecoder) throws -> SupervisedEstimatorToTemporalAdaptor&lt;Base>.Transformer

Decodes the transformer.

### Fitting

func fitted&lt;InputSequence, FeatureSequence>(to: InputSequence, eventHandler: EventHandler?) async throws -> SupervisedEstimatorToTemporalAdaptor&lt;Base>.Transformer

Fits a transformer to a sequence of examples.

func fitted&lt;InputSequence, Validation, FeatureSequence>(to: InputSequence, validateOn: Validation, eventHandler: EventHandler?) async throws -> SupervisedEstimatorToTemporalAdaptor&lt;Base>.Transformer

Fits a transformer to a sequence of examples while validating with a validation sequence.

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

## Relationships

### Conforms To

- Sendable
- SupervisedTemporalEstimator

## See Also

### Estimator adaptors

struct EstimatorToSupervisedAdaptor

An adaptor that exposes an estimator as a supervised estimator.

struct EstimatorToTemporalAdaptor

A temporal estimator wrapping an estimator.

Deprecated

