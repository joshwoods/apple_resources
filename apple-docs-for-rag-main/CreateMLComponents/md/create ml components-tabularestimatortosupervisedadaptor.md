

- Create ML Components
-  TabularEstimatorToSupervisedAdaptor 

Structure

# TabularEstimatorToSupervisedAdaptor

An adaptor that exposes a tabular estimator as a tabular supervised estimator.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct TabularEstimatorToSupervisedAdaptor where Estimator : TabularEstimator
```

## Topics

### Creating an adaptor

init(Estimator, annotationColumnID: ColumnID&lt;Annotation>)

Creates a tabular estimator supervised adaptor.

### Getting the properties

var annotationColumnID: ColumnID&lt;Annotation>

The annotation column identifier.

let estimator: Estimator

The wrapped estimator.

### Encoding and decoding

func encode(Estimator.Transformer, to: inout any EstimatorEncoder) throws

Encodes a fitted transformer.

func decode(from: inout any EstimatorDecoder) throws -> Estimator.Transformer

Decodes a previously fitted transformer.

### Fitting

func fitted(to: DataFrame, validateOn: DataFrame?, eventHandler: EventHandler?) async throws -> Estimator.Transformer

Returns the tabular transformer fitted using the provided tabular estimator.

typealias Transformer

The transformer type created by this estimator.

### Default Implementations

SupervisedTabularEstimator Implementations

## Relationships

### Conforms To

- Sendable
- SupervisedTabularEstimator

## See Also

### Tabular adaptors

struct TabularTransformerToEstimatorAdaptor

A tabular estimator that always returns a predefined tabular transformer.

struct TabularTransformerToUpdatableEstimatorAdaptor

An updatable tabular estimator that always returns a predefined transformer.

struct UpdatableTabularEstimatorToSupervisedAdaptor

An adaptor that exposes an updatable tabular estimator as an updatable supervised tabular estimator.

