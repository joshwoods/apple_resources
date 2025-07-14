

- Create ML Components
- PreprocessingSupervisedEstimator
-  fitted(toPreprocessed:validateOn:eventHandler:) 

Instance Method

# fitted(toPreprocessed:validateOn:eventHandler:)

Fits a composed transformer to a sequence of preprocessed features.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func fitted(
    toPreprocessed preprocessedInput: Input,
    validateOn preprocessedValidation: Validation,
    eventHandler: EventHandler? = nil
) async throws -> PreprocessingSupervisedEstimator.Transformer where Input : Sequence, Validation : Sequence, Input.Element == AnnotatedFeature, Validation.Element == AnnotatedFeature
```

## Parameters 

`preprocessedInput`  

A sequence of preprocessed features.

`preprocessedValidation`  

A sequence of preprocessed features used for validating the fitted transformer.

`eventHandler`  

An event handler.

## Return Value

The fitted transformer.

## See Also

### Preprocessing and fitting

func preprocessed&lt;S>(from: S, eventHandler: EventHandler?) async throws -> AnySequence&lt;AnnotatedFeature&lt;Preprocessor.Output, PreprocessingSupervisedEstimator&lt;Preprocessor, Estimator>.Annotation>>

Preprocesses a sequence of examples.

func fitted&lt;InputSequence>(to: InputSequence, eventHandler: EventHandler?) async throws -> PreprocessingSupervisedEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a composed transformer to a sequence of examples.

func fitted&lt;S>(toPreprocessed: S, eventHandler: EventHandler?) async throws -> PreprocessingSupervisedEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a transformer to a sequence of preprocessed features.

func fitted&lt;InputSequence, Validation>(to: InputSequence, validateOn: Validation, eventHandler: EventHandler?) async throws -> PreprocessingSupervisedEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a composed transformer to a sequence of examples.

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

