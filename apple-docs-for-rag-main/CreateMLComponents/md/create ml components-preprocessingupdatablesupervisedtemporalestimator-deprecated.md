

- Create ML Components
-  PreprocessingUpdatableSupervisedTemporalEstimator Deprecated

Structure

# PreprocessingUpdatableSupervisedTemporalEstimator

An updatable supervised temporal estimator that composes a preprocessing transformer and an updatable supervised temporal estimator.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
struct PreprocessingUpdatableSupervisedTemporalEstimator where Preprocessor : TemporalTransformer, Estimator : UpdatableSupervisedTemporalEstimator, Preprocessor.Output == Estimator.Transformer.Input
```

## Topics

### Creating an estimator

init(Preprocessor, Estimator)

Creates a composed supervised temporal estimator from a preprocessing transformer and a supervised temporal estimator.

### Getting the properties

var estimator: Estimator

The estimator.

var preprocessor: Preprocessor

The preprocessing transformer.

### Encoding and decoding

func encode(PreprocessingUpdatableSupervisedTemporalEstimator&lt;Preprocessor, Estimator>.Transformer, to: inout any EstimatorEncoder) throws

Encodes a fitted transformer.

func decode(from: inout any EstimatorDecoder) throws -> PreprocessingUpdatableSupervisedTemporalEstimator&lt;Preprocessor, Estimator>.Transformer

Decodes a previously fitted transformer.

func decodeWithOptimizer(from: inout any EstimatorDecoder) throws -> PreprocessingUpdatableSupervisedTemporalEstimator&lt;Preprocessor, Estimator>.Transformer

Reads the encoded transformer and optimizer with a decoder.

func encodeWithOptimizer(PreprocessingUpdatableSupervisedTemporalEstimator&lt;Preprocessor, Estimator>.Transformer, to: inout any EstimatorEncoder) throws

Encodes the transformer and optimizer to an encoder.

### Preprocesing and fitting

func preprocessed&lt;InputSequence, FeatureSequence>(from: InputSequence, eventHandler: EventHandler?) async throws -> [AnnotatedFeature&lt;PreprocessedFeatureSequence&lt;Preprocessor.Output>, PreprocessingUpdatableSupervisedTemporalEstimator&lt;Preprocessor, Estimator>.Annotation>]

Preprocesses a sequence of examples.

func fitted&lt;InputSequence, FeatureSequence>(to: InputSequence, eventHandler: EventHandler?) async throws -> PreprocessingUpdatableSupervisedTemporalEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a transformer to a sequence of examples.

func fitted(toPreprocessed: [AnnotatedFeature&lt;PreprocessedFeatureSequence&lt;Preprocessor.Output>, PreprocessingUpdatableSupervisedTemporalEstimator&lt;Preprocessor, Estimator>.Annotation>], eventHandler: EventHandler?) async throws -> PreprocessingUpdatableSupervisedTemporalEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a transformer to a sequence of preprocessed features.

func fitted&lt;InputSequence, Validation, FeatureSequence>(to: InputSequence, validateOn: Validation, eventHandler: EventHandler?) async throws -> PreprocessingUpdatableSupervisedTemporalEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a transformer to a sequence of examples while validating with a validation sequence.

func fitted(toPreprocessed: [AnnotatedFeature&lt;PreprocessedFeatureSequence&lt;Preprocessor.Output>, PreprocessingUpdatableSupervisedTemporalEstimator&lt;Preprocessor, Estimator>.Annotation>], validateOn: [AnnotatedFeature&lt;PreprocessedFeatureSequence&lt;Preprocessor.Output>, PreprocessingUpdatableSupervisedTemporalEstimator&lt;Preprocessor, Estimator>.Annotation>], eventHandler: EventHandler?) async throws -> PreprocessingUpdatableSupervisedTemporalEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a transformer to a sequence of preprocessed features while validating.

func makeTransformer() -> PreprocessingUpdatableSupervisedTemporalEstimator&lt;Preprocessor, Estimator>.Transformer

Creates a default-initialized transformer suitable for incremental fitting.

func update&lt;InputSequence, FeatureSequence>(inout PreprocessingUpdatableSupervisedTemporalEstimator&lt;Preprocessor, Estimator>.Transformer, with: InputSequence, eventHandler: EventHandler?) async throws

Updates a transformer with a new sequence of examples.

func update&lt;InputSequence, FeatureSequence>(inout PreprocessingUpdatableSupervisedTemporalEstimator&lt;Preprocessor, Estimator>.Transformer, withPreprocessed: InputSequence, eventHandler: EventHandler?) async throws

Updates a transformer with a new sequence of preprocessed features.

typealias Annotation

The annotation type.

typealias Input

The input type.

typealias Intermediate

The intermediate type.

typealias Output

The output type.

typealias Transformer

The transformer type created by this estimator.

### Default Implementations

SupervisedTemporalEstimator Implementations

UpdatableSupervisedTemporalEstimator Implementations

## Relationships

### Conforms To

- Sendable
- SupervisedTemporalEstimator
- UpdatableSupervisedTemporalEstimator

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

struct PreprocessingUpdatableTemporalEstimator

An updatable temporal estimator that composes a preprocessing transformer and an updatable temporal estimator.

Deprecated

struct PreprocessingUpdatableSupervisedEstimator

An updatable supervised estimator that composes a preprocessing transformer and an updatable supervised estimator.

