

- Create ML Components
- PreprocessingSupervisedTemporalEstimator
-  preprocessed(from:eventHandler:) Deprecated

Instance Method

# preprocessed(from:eventHandler:)

Preprocesses a sequence of examples.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func preprocessed(
    from input: InputSequence,
    eventHandler: EventHandler? = nil
) async throws -> [AnnotatedFeature, PreprocessingSupervisedTemporalEstimator.Annotation>] where InputSequence : Sequence, FeatureSequence : TemporalSequence, Preprocessor.Input == FeatureSequence.Feature, InputSequence.Element == AnnotatedFeature
```

## Parameters 

`input`  

A sequence of examples.

`eventHandler`  

An event handler.

## Return Value

The preprocessed examples.

## See Also

### Preprocesing and Fitting

func fitted&lt;InputSequence, FeatureSequence>(to: InputSequence, eventHandler: EventHandler?) async throws -> PreprocessingSupervisedTemporalEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a transformer to a sequence of examples.

Deprecated

func fitted(toPreprocessed: [AnnotatedFeature&lt;PreprocessedFeatureSequence&lt;Preprocessor.Output>, PreprocessingSupervisedTemporalEstimator&lt;Preprocessor, Estimator>.Annotation>], eventHandler: EventHandler?) async throws -> PreprocessingSupervisedTemporalEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a transformer to a sequence of preprocessed annotated features.

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

