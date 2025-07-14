

- Create ML Components
-  PreprocessingUpdatableEstimator 

Structure

# PreprocessingUpdatableEstimator

An updatable estimator that composes a preprocessing transformer and an updatable estimator.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct PreprocessingUpdatableEstimator where Preprocessor : Transformer, Estimator : UpdatableEstimator, Preprocessor.Output == Estimator.Transformer.Input
```

## Topics

### Creating an estimator

init(Preprocessor, Estimator)

Creates a composed updatable estimator from a preprocessing transformer and an estimator.

### Getting the properties

var estimator: Estimator

The estimator.

var preprocessor: Preprocessor

The preprocessing transformer.

### Encoding and decoding

func encode(PreprocessingUpdatableEstimator&lt;Preprocessor, Estimator>.Transformer, to: inout any EstimatorEncoder) throws

Encodes a fitted transformer.

func decode(from: inout any EstimatorDecoder) throws -> PreprocessingUpdatableEstimator&lt;Preprocessor, Estimator>.Transformer

Decodes a previously fitted transformer.

func decodeWithOptimizer(from: inout any EstimatorDecoder) throws -> PreprocessingUpdatableEstimator&lt;Preprocessor, Estimator>.Transformer

Reads the encoded transformer and optimizer.

func encodeWithOptimizer(PreprocessingUpdatableEstimator&lt;Preprocessor, Estimator>.Transformer, to: inout any EstimatorEncoder) throws

Encodes the transformer and optimizer to an encoder.

### Preprocesing and fitting

func preprocessed&lt;S>(from: S, eventHandler: EventHandler?) async throws -> [Preprocessor.Output]

Preprocesses a sequence of examples.

func fitted&lt;S>(to: S, eventHandler: EventHandler?) async throws -> PreprocessingUpdatableEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a composed transformer to a sequence of examples.

func fitted&lt;S>(toPreprocessed: S, eventHandler: EventHandler?) async throws -> PreprocessingUpdatableEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a transformer to a sequence of preprocessed features.

func makeTransformer() -> PreprocessingUpdatableEstimator&lt;Preprocessor, Estimator>.Transformer

Creates a default-initialized transformer suitable for incremental fitting.

func update&lt;InputSequence>(inout PreprocessingUpdatableEstimator&lt;Preprocessor, Estimator>.Transformer, with: InputSequence, eventHandler: EventHandler?) async throws

Updates a transformer with a new sequence of examples.

func update&lt;InputSequence>(inout PreprocessingUpdatableEstimator&lt;Preprocessor, Estimator>.Transformer, withPreprocessed: InputSequence, eventHandler: EventHandler?) async throws

Updates a transformer with a new sequence of preprocessed features.

typealias Input

The input type.

typealias Intermediate

The intermediate type.

typealias Output

The output type.

typealias Transformer

The transformer type created by this estimator.

### Default Implementations

Estimator Implementations

UpdatableEstimator Implementations

## Relationships

### Conforms To

- Estimator
- Sendable
- UpdatableEstimator

## See Also

### Composition with preprocessing

struct PreprocessingEstimator

An estimator that composes a preprocessing transformer and an estimator.

struct PreprocessingTemporalEstimator

A temporal estimator that composes a preprocessing transformer and a temporal estimator.

Deprecated

struct PreprocessingSupervisedEstimator

A supervised estimator that composes a preprocessing transformer and a supervised estimator.

struct PreprocessingSupervisedTemporalEstimator

A supervised temporal estimator that composes a preprocessing transformer and a supervised temporal estimator.

Deprecated

struct PreprocessingUpdatableTemporalEstimator

An updatable temporal estimator that composes a preprocessing transformer and an updatable temporal estimator.

Deprecated

struct PreprocessingUpdatableSupervisedEstimator

An updatable supervised estimator that composes a preprocessing transformer and an updatable supervised estimator.

struct PreprocessingUpdatableSupervisedTemporalEstimator

An updatable supervised temporal estimator that composes a preprocessing transformer and an updatable supervised temporal estimator.

Deprecated

