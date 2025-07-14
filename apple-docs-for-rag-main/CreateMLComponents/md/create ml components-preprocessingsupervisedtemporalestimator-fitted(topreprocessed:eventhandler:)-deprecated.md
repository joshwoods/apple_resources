

- Create ML Components
- PreprocessingSupervisedTemporalEstimator
-  fitted(toPreprocessed:eventHandler:) Deprecated

Instance Method

# fitted(toPreprocessed:eventHandler:)

Fits a transformer to a sequence of preprocessed annotated features.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func fitted(
    toPreprocessed preprocessed: [AnnotatedFeature, PreprocessingSupervisedTemporalEstimator.Annotation>],
    eventHandler: EventHandler? = nil
) async throws -> PreprocessingSupervisedTemporalEstimator.Transformer
```

## Parameters 

`preprocessed`  

A sequence of preprocessed features.

`eventHandler`  

An event handler.

## Return Value

The fitted transformer.

## See Also

### Preprocesing and Fitting

func preprocessed&lt;InputSequence, FeatureSequence>(from: InputSequence, eventHandler: EventHandler?) async throws -> [AnnotatedFeature&lt;PreprocessedFeatureSequence&lt;Preprocessor.Output>, PreprocessingSupervisedTemporalEstimator&lt;Preprocessor, Estimator>.Annotation>]

Preprocesses a sequence of examples.

Deprecated

func fitted&lt;InputSequence, FeatureSequence>(to: InputSequence, eventHandler: EventHandler?) async throws -> PreprocessingSupervisedTemporalEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a transformer to a sequence of examples.

Deprecated

func fitted&lt;InputSequence, Validation, FeatureSequence>(to: InputSequence, validateOn: Validation, eventHandler: EventHandler?) async throws -> PreprocessingSupervisedTemporalEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a transformer to a sequence of examples while validating with a validation sequence.

Deprecated

func fitted(toPreprocessed: [AnnotatedFeature&lt;PreprocessedFeatureSequence&lt;Preprocessor.Output>, PreprocessingSupervisedTemporalEstimator&lt;Preprocessor, Estimator>.Annotation>], validateOn: [AnnotatedFeature&lt;PreprocessedFeatureSequence&lt;Preprocessor.Output>, PreprocessingSupervisedTemporalEstimator&lt;Preprocessor, Estimator>.Annotation>], eventHandler: EventHandler?) async throws -> PreprocessingSupervisedTemporalEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a transformer to a sequence of preprocessed examples while validating.

Deprecated

typealias Annotation

The annotation type.

Deprecated

typealias Input

The input type.

Deprecated

typealias Intermediate

The intermediate type.

Deprecated

typealias Output

The output type.

Deprecated

typealias Transformer

The transformer type created by this estimator.

Deprecated

