

- Create ML Components
-  TemporalEstimatorToSupervisedAdaptor Deprecated

Structure

# TemporalEstimatorToSupervisedAdaptor

An adaptor that exposes a temporal estimator as a supervised temporal estimator.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
struct TemporalEstimatorToSupervisedAdaptor where Estimator : TemporalEstimator, Annotation : Equatable, Annotation : Sendable
```

## Topics

### Creating an adaptor

init(Estimator)

Creates a temporal estimator adaptor.

### Getting the estimator

let estimator: Estimator

The wrapped estimator.

### Encoding and decoding

func encode(TemporalEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer, to: inout any EstimatorEncoder) throws

Does nothing since this estimator uses a pre-defined transformer.

func decode(from: inout any EstimatorDecoder) throws -> TemporalEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer

Returns the pre-defined transformer.

### Fitting

func fitted&lt;InputSequence, FeatureSequence>(to: InputSequence, eventHandler: EventHandler?) async throws -> TemporalEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer

Fits a transformer to a sequence of examples.

func fitted&lt;InputSequence, Validation, FeatureSequence>(to: InputSequence, validateOn: Validation, eventHandler: EventHandler?) async throws -> TemporalEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer

Fits a transformer to a sequence of examples while validating with a validation sequence.

typealias Transformer

The transformer type created by this estimator.

### Default Implementations

SupervisedTemporalEstimator Implementations

## Relationships

### Conforms To

- Sendable
- SupervisedTemporalEstimator

## See Also

### Temporal adaptors

struct TemporalAdaptor

A temporal transformer that applies a regular transformer to each value of a temporal sequence.

struct TemporalTransformerToEstimatorAdaptor

A temporal estimator that always returns a predefined temporal transformer.

Deprecated

struct TemporalTransformerToUpdatableEstimatorAdaptor

A temporal estimator that always returns a predefined temporal transformer.

Deprecated

