

- Create ML Components
- PreprocessingUpdatableSupervisedEstimator
-  preprocessed(from:eventHandler:) 

Instance Method

# preprocessed(from:eventHandler:)

Preprocesses a sequence of examples.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func preprocessed(
    from input: S,
    eventHandler: EventHandler? = nil
) async throws -> AnySequence.Annotation>> where S : Sequence, S.Element == AnnotatedFeature
```

## Parameters 

`input`  

A sequence of examples.

`eventHandler`  

An event handler.

## Return Value

The preprocessed examples.

## See Also

### Preprocesing and fitting

func fitted&lt;InputSequence>(to: InputSequence, eventHandler: EventHandler?) async throws -> PreprocessingUpdatableSupervisedEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a composed transformer to a sequence of examples.

func fitted&lt;S>(toPreprocessed: S, eventHandler: EventHandler?) async throws -> PreprocessingUpdatableSupervisedEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a transformer to a sequence of preprocessed features.

func fitted&lt;InputSequence, Validation>(to: InputSequence, validateOn: Validation, eventHandler: EventHandler?) async throws -> PreprocessingUpdatableSupervisedEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a composed transformer to a sequence of examples.

func fitted&lt;InputSequence, Validation>(toPreprocessed: InputSequence, validateOn: Validation, eventHandler: EventHandler?) async throws -> PreprocessingUpdatableSupervisedEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a composed transformer to a sequence of examples.

func makeTransformer() -> PreprocessingUpdatableSupervisedEstimator&lt;Preprocessor, Estimator>.Transformer

Creates a default-initialized transformer suitable for incremental fitting.

func update&lt;InputSequence>(inout PreprocessingUpdatableSupervisedEstimator&lt;Preprocessor, Estimator>.Transformer, with: InputSequence, eventHandler: EventHandler?) async throws

Updates a transformer with a new sequence of examples.

func update&lt;InputSequence>(inout PreprocessingUpdatableSupervisedEstimator&lt;Preprocessor, Estimator>.Transformer, withPreprocessed: InputSequence, eventHandler: EventHandler?) async throws

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

