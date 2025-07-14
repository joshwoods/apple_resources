

- Create ML Components
-  TransformerToUpdatableEstimatorAdaptor 

Structure

# TransformerToUpdatableEstimatorAdaptor

An updatable estimator that always returns a predefined transformer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct TransformerToUpdatableEstimatorAdaptor where Transformer : Transformer
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

Does nothing since this estimator uses a pre-defined transformer.

func decodeWithOptimizer(from: inout any EstimatorDecoder) throws -> Transformer

Returns the pre-defined transformer.

### Fitting and updating

func fitted&lt;S>(to: S, eventHandler: EventHandler?) async throws -> Transformer

Returns the pre-defined transformer.

func makeTransformer() -> Transformer

Creates a default-initialized transformer suitable for incremental fitting.

func update&lt;InputSequence>(inout Transformer, with: InputSequence, eventHandler: EventHandler?) async throws

Does nothing since this estimator uses a pre-defined transformer.

### Default Implementations

Estimator Implementations

UpdatableEstimator Implementations

## Relationships

### Conforms To

- Estimator
- Sendable
- UpdatableEstimator

## See Also

### Transformer adaptors

struct TransformerToEstimatorAdaptor

An estimator that always returns a predefined transformer.

struct TransformerToTemporalAdaptor

A temporal transformer that applies a regular transformer to each value of a temporal sequence.

Deprecated

