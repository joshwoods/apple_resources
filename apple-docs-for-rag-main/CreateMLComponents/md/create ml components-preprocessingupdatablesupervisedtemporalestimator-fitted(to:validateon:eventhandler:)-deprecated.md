

- Create ML Components
- PreprocessingUpdatableSupervisedTemporalEstimator
-  fitted(to:validateOn:eventHandler:) Deprecated

Instance Method

# fitted(to:validateOn:eventHandler:)

Fits a transformer to a sequence of examples while validating with a validation sequence.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func fitted(
    to input: InputSequence,
    validateOn validation: Validation,
    eventHandler: EventHandler? = nil
) async throws -> PreprocessingUpdatableSupervisedTemporalEstimator.Transformer where InputSequence : Sequence, Validation : Sequence, FeatureSequence : TemporalSequence, Preprocessor.Input == FeatureSequence.Feature, InputSequence.Element == AnnotatedFeature, Validation.Element == AnnotatedFeature
```

## Parameters 

`input`  

A sequence of examples used for fitting the transformer.

`validation`  

A sequence of examples used for validating the fitted transformer.

`eventHandler`  

An event handler.

## Return Value

The fitted transformer.

## See Also

### Preprocesing and fitting

func preprocessed&lt;InputSequence, FeatureSequence>(from: InputSequence, eventHandler: EventHandler?) async throws -> [AnnotatedFeature&lt;PreprocessedFeatureSequence&lt;Preprocessor.Output>, PreprocessingUpdatableSupervisedTemporalEstimator&lt;Preprocessor, Estimator>.Annotation>]

Preprocesses a sequence of examples.

Deprecated

func fitted&lt;InputSequence, FeatureSequence>(to: InputSequence, eventHandler: EventHandler?) async throws -> PreprocessingUpdatableSupervisedTemporalEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a transformer to a sequence of examples.

Deprecated

func fitted(toPreprocessed: [AnnotatedFeature&lt;PreprocessedFeatureSequence&lt;Preprocessor.Output>, PreprocessingUpdatableSupervisedTemporalEstimator&lt;Preprocessor, Estimator>.Annotation>], eventHandler: EventHandler?) async throws -> PreprocessingUpdatableSupervisedTemporalEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a transformer to a sequence of preprocessed features.

Deprecated

func fitted(toPreprocessed: [AnnotatedFeature&lt;PreprocessedFeatureSequence&lt;Preprocessor.Output>, PreprocessingUpdatableSupervisedTemporalEstimator&lt;Preprocessor, Estimator>.Annotation>], validateOn: [AnnotatedFeature&lt;PreprocessedFeatureSequence&lt;Preprocessor.Output>, PreprocessingUpdatableSupervisedTemporalEstimator&lt;Preprocessor, Estimator>.Annotation>], eventHandler: EventHandler?) async throws -> PreprocessingUpdatableSupervisedTemporalEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a transformer to a sequence of preprocessed features while validating.

Deprecated

func makeTransformer() -> PreprocessingUpdatableSupervisedTemporalEstimator&lt;Preprocessor, Estimator>.Transformer

Creates a default-initialized transformer suitable for incremental fitting.

Deprecated

func update&lt;InputSequence, FeatureSequence>(inout PreprocessingUpdatableSupervisedTemporalEstimator&lt;Preprocessor, Estimator>.Transformer, with: InputSequence, eventHandler: EventHandler?) async throws

Updates a transformer with a new sequence of examples.

Deprecated

func update&lt;InputSequence, FeatureSequence>(inout PreprocessingUpdatableSupervisedTemporalEstimator&lt;Preprocessor, Estimator>.Transformer, withPreprocessed: InputSequence, eventHandler: EventHandler?) async throws

Updates a transformer with a new sequence of preprocessed features.

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

