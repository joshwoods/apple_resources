

- Create ML Components
-  PreprocessingUpdatableTemporalEstimator Deprecated

Structure

# PreprocessingUpdatableTemporalEstimator

An updatable temporal estimator that composes a preprocessing transformer and an updatable temporal estimator.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
struct PreprocessingUpdatableTemporalEstimator where Preprocessor : TemporalTransformer, Estimator : UpdatableTemporalEstimator, Preprocessor.Output == Estimator.Transformer.Input
```

## Topics

### Creating an estimator

init(Preprocessor, Estimator)

Creates a composed temporal estimator from a preprocessing transformer and a temporal estimator.

### Getting the properties

var estimator: Estimator

The estimator.

var preprocessor: Preprocessor

The preprocessing transformer.

### Encoding and decoding

func encode(PreprocessingUpdatableTemporalEstimator&lt;Preprocessor, Estimator>.Transformer, to: inout any EstimatorEncoder) throws

Encodes a fitted transformer.

func decode(from: inout any EstimatorDecoder) throws -> PreprocessingUpdatableTemporalEstimator&lt;Preprocessor, Estimator>.Transformer

Decodes a previously fitted transformer.

func encodeWithOptimizer(PreprocessingUpdatableTemporalEstimator&lt;Preprocessor, Estimator>.Transformer, to: inout any EstimatorEncoder) throws

Encodes the transformer and optimizer to an encoder.

func decodeWithOptimizer(from: inout any EstimatorDecoder) throws -> PreprocessingUpdatableTemporalEstimator&lt;Preprocessor, Estimator>.Transformer

Reads the encoded transformer and optimizer with a decoder.

### Preprocesing and fitting

func preprocessed&lt;InputSequence>(from: InputSequence, eventHandler: EventHandler?) async throws -> [PreprocessedFeatureSequence&lt;Preprocessor.Output>]

Preprocesses a sequence of examples.

func fitted&lt;InputSequence>(to: InputSequence, eventHandler: EventHandler?) async throws -> PreprocessingUpdatableTemporalEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a transformer to a sequence of examples.

func fitted(toPreprocessed: [PreprocessedFeatureSequence&lt;Preprocessor.Output>], eventHandler: EventHandler?) async throws -> PreprocessingUpdatableTemporalEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a transformer to a sequence of preprocessed features.

func update&lt;InputSequence>(inout PreprocessingUpdatableTemporalEstimator&lt;Preprocessor, Estimator>.Transformer, withPreprocessed: InputSequence, eventHandler: EventHandler?) async throws

Updates a transformer with a new sequence of preprocessed features.

func update&lt;InputSequence>(inout PreprocessingUpdatableTemporalEstimator&lt;Preprocessor, Estimator>.Transformer, with: InputSequence, eventHandler: EventHandler?) async throws

Updates a transformer with a new sequence of examples.

func makeTransformer() -> PreprocessingUpdatableTemporalEstimator&lt;Preprocessor, Estimator>.Transformer

Creates a default-initialized transformer suitable for incremental fitting.

typealias Input

The input type.

typealias Intermediate

The intermediate type.

typealias Output

The output type.

typealias Transformer

The transformer type created by this estimator.

### Default Implementations

TemporalEstimator Implementations

UpdatableTemporalEstimator Implementations

## Relationships

### Conforms To

- Sendable
- TemporalEstimator
- UpdatableTemporalEstimator

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

struct PreprocessingUpdatableEstimator

An updatable estimator that composes a preprocessing transformer and an updatable estimator.

struct PreprocessingUpdatableSupervisedEstimator

An updatable supervised estimator that composes a preprocessing transformer and an updatable supervised estimator.

struct PreprocessingUpdatableSupervisedTemporalEstimator

An updatable supervised temporal estimator that composes a preprocessing transformer and an updatable supervised temporal estimator.

Deprecated

