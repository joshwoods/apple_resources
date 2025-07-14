

- Create ML Components
-  UpdatableTabularEstimatorToSupervisedAdaptor 

Structure

# UpdatableTabularEstimatorToSupervisedAdaptor

An adaptor that exposes an updatable tabular estimator as an updatable supervised tabular estimator.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct UpdatableTabularEstimatorToSupervisedAdaptor where Estimator : UpdatableTabularEstimator, Annotation : Equatable
```

## Topics

### Creating an adaptor

init(Estimator, annotationColumnID: ColumnID&lt;Annotation>)

Creates an updatable tabular estimator supervised adaptor.

### Getting the properties

var annotationColumnID: ColumnID&lt;Annotation>

The annotation column identifier.

let estimator: Estimator

The wrapped estimator.

### Encoding and decoding

func encode(UpdatableTabularEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer, to: inout any EstimatorEncoder) throws

Does nothing since this estimator uses a pre-defined transformer.

func decode(from: inout any EstimatorDecoder) throws -> UpdatableTabularEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer

Returns the pre-defined transformer.

func encodeWithOptimizer(UpdatableTabularEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer, to: inout any EstimatorEncoder) throws

Encodes the transformer and optimizer to an encoder.

func decodeWithOptimizer(from: inout any EstimatorDecoder) throws -> UpdatableTabularEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer

Reads the encoded transformer and optimizer.

### Fitting

func fitted(to: DataFrame, validateOn: DataFrame?, eventHandler: EventHandler?) async throws -> UpdatableTabularEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer

Fits a transformer to a data frame.

func makeTransformer() -> Estimator.Transformer

Creates a default-initialized transformer suitable for incremental fitting.

func update(inout UpdatableTabularEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer, with: DataFrame, eventHandler: EventHandler?) async throws

Updates a transformer with a new data frame containing examples.

typealias Transformer

The transformer type created by this estimator.

### Default Implementations

SupervisedTabularEstimator Implementations

UpdatableSupervisedTabularEstimator Implementations

## Relationships

### Conforms To

- Sendable
- SupervisedTabularEstimator
- UpdatableSupervisedTabularEstimator

## See Also

### Tabular adaptors

struct TabularEstimatorToSupervisedAdaptor

An adaptor that exposes a tabular estimator as a tabular supervised estimator.

struct TabularTransformerToEstimatorAdaptor

A tabular estimator that always returns a predefined tabular transformer.

struct TabularTransformerToUpdatableEstimatorAdaptor

An updatable tabular estimator that always returns a predefined transformer.

