

- Create ML Components
-  TransformerToEstimatorAdaptor 

Structure

# TransformerToEstimatorAdaptor

An estimator that always returns a predefined transformer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct TransformerToEstimatorAdaptor where Transformer : Transformer
```

## Topics

### Creating a feature

init(Transformer)

Creates a trivial estimator.

### Getting the transformer

let transformer: Transformer

A pre-defined transformer.

### Encoding and Decoding

func encode(Transformer, to: inout any EstimatorEncoder) throws

Does nothing since this estimator uses a pre-defined transformer.

func decode(from: inout any EstimatorDecoder) throws -> Transformer

Returns the pre-defined transformer.

### Fitting

func fitted&lt;S>(to: S, eventHandler: EventHandler?) async throws -> Transformer

Returns the pre-defined transformer.

### Default Implementations

Estimator Implementations

## Relationships

### Conforms To

- Estimator
- Sendable

## See Also

### Transformer adaptors

struct TransformerToTemporalAdaptor

A temporal transformer that applies a regular transformer to each value of a temporal sequence.

Deprecated

struct TransformerToUpdatableEstimatorAdaptor

An updatable estimator that always returns a predefined transformer.

