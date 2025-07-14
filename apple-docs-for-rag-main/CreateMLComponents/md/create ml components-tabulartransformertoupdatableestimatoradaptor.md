

- Create ML Components
-  TabularTransformerToUpdatableEstimatorAdaptor 

Structure

# TabularTransformerToUpdatableEstimatorAdaptor

An updatable tabular estimator that always returns a predefined transformer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct TabularTransformerToUpdatableEstimatorAdaptor where Transformer : TabularTransformer
```

## Topics

### Creating an estimator

init(Transformer)

Creates an updatable tabular estimator from a tabular transformer.

### Creating a default transformer

func makeTransformer() -> Transformer

Creates a default-initialized transformer suitable for incremental fitting.

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

### Fitting

func fitted(to: DataFrame, eventHandler: EventHandler?) async throws -> Transformer

Returns the pre-defined transformer.

func update(inout Transformer, with: DataFrame, eventHandler: EventHandler?) async throws

Does nothing since this estimator uses a pre-defined transformer.

### Default Implementations

TabularEstimator Implementations

UpdatableTabularEstimator Implementations

## Relationships

### Conforms To

- Sendable
- TabularEstimator
- UpdatableTabularEstimator

## See Also

### Tabular adaptors

struct TabularEstimatorToSupervisedAdaptor

An adaptor that exposes a tabular estimator as a tabular supervised estimator.

struct TabularTransformerToEstimatorAdaptor

A tabular estimator that always returns a predefined tabular transformer.

struct UpdatableTabularEstimatorToSupervisedAdaptor

An adaptor that exposes an updatable tabular estimator as an updatable supervised tabular estimator.

