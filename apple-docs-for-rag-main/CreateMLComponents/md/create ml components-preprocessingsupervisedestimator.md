

- Create ML Components
-  PreprocessingSupervisedEstimator 

Structure

# PreprocessingSupervisedEstimator

A supervised estimator that composes a preprocessing transformer and a supervised estimator.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct PreprocessingSupervisedEstimator where Preprocessor : Transformer, Estimator : SupervisedEstimator, Preprocessor.Output == Estimator.Transformer.Input
```

## Topics

### Creating the estimator

init(Preprocessor, Estimator)

Creates a composed supervised estimator from a preprocessing transformer and an estimator.

### Getting the properties

var estimator: Estimator

The estimator.

var preprocessor: Preprocessor

The preprocessing transformer.

### Encoding and decoding

func encode(PreprocessingSupervisedEstimator&lt;Preprocessor, Estimator>.Transformer, to: inout any EstimatorEncoder) throws

Encodes a fitted transformer.

func decode(from: inout any EstimatorDecoder) throws -> PreprocessingSupervisedEstimator&lt;Preprocessor, Estimator>.Transformer

Decodes a previously fitted transformer.

### Preprocessing and fitting

func preprocessed&lt;S>(from: S, eventHandler: EventHandler?) async throws -> AnySequence&lt;AnnotatedFeature&lt;Preprocessor.Output, PreprocessingSupervisedEstimator&lt;Preprocessor, Estimator>.Annotation>>

Preprocesses a sequence of examples.

func fitted&lt;InputSequence>(to: InputSequence, eventHandler: EventHandler?) async throws -> PreprocessingSupervisedEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a composed transformer to a sequence of examples.

func fitted&lt;S>(toPreprocessed: S, eventHandler: EventHandler?) async throws -> PreprocessingSupervisedEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a transformer to a sequence of preprocessed features.

func fitted&lt;InputSequence, Validation>(to: InputSequence, validateOn: Validation, eventHandler: EventHandler?) async throws -> PreprocessingSupervisedEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a composed transformer to a sequence of examples.

func fitted&lt;Input, Validation>(toPreprocessed: Input, validateOn: Validation, eventHandler: EventHandler?) async throws -> PreprocessingSupervisedEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a composed transformer to a sequence of preprocessed features.

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

SupervisedEstimator Implementations

## Relationships

### Conforms To

- Sendable
- SupervisedEstimator

## See Also

### Composition with preprocessing

struct PreprocessingEstimator

An estimator that composes a preprocessing transformer and an estimator.

struct PreprocessingTemporalEstimator

A temporal estimator that composes a preprocessing transformer and a temporal estimator.

Deprecated

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

struct PreprocessingUpdatableSupervisedTemporalEstimator

An updatable supervised temporal estimator that composes a preprocessing transformer and an updatable supervised temporal estimator.

Deprecated

