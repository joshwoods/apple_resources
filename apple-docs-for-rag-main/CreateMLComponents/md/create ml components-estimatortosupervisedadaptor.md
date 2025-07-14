

- Create ML Components
-  EstimatorToSupervisedAdaptor 

Structure

# EstimatorToSupervisedAdaptor

An adaptor that exposes an estimator as a supervised estimator.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct EstimatorToSupervisedAdaptor where Estimator : Estimator, Annotation : Equatable
```

## Topics

### Creating the adaptor

init(Estimator)

Creates an estimator adaptor.

### Getting the properties

let estimator: Estimator

The wrapped estimator.

### Encoding and decoding

func encode(EstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer, to: inout any EstimatorEncoder) throws

Does nothing since this estimator uses a pre-defined transformer.

func decode(from: inout any EstimatorDecoder) throws -> EstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer

Returns the pre-defined transformer.

### Fitting a transformer

func fitted&lt;Input>(to: Input, eventHandler: EventHandler?) async throws -> EstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer

Fits a transformer to a sequence of examples, ignoring the annotations and the validation.

func fitted&lt;Input, Validation>(to: Input, validateOn: Validation, eventHandler: EventHandler?) async throws -> EstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer

Fits a transformer to a sequence of examples.

typealias Transformer

The transformer type created by this estimator.

### Default Implementations

SupervisedEstimator Implementations

## Relationships

### Conforms To

- Sendable
- SupervisedEstimator

## See Also

### Estimator adaptors

struct EstimatorToTemporalAdaptor

A temporal estimator wrapping an estimator.

Deprecated

struct SupervisedEstimatorToTemporalAdaptor

A supervised temporal estimator wrapping a supervised estimator.

Deprecated

