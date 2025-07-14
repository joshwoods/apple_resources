

- Create ML Components
- PreprocessingUpdatableSupervisedTemporalEstimator
-  makeTransformer() Deprecated

Instance Method

# makeTransformer()

Creates a default-initialized transformer suitable for incremental fitting.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func makeTransformer() -> PreprocessingUpdatableSupervisedTemporalEstimator.Transformer
```

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

func fitted&lt;InputSequence, Validation, FeatureSequence>(to: InputSequence, validateOn: Validation, eventHandler: EventHandler?) async throws -> PreprocessingUpdatableSupervisedTemporalEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a transformer to a sequence of examples while validating with a validation sequence.

Deprecated

func fitted(toPreprocessed: [AnnotatedFeature&lt;PreprocessedFeatureSequence&lt;Preprocessor.Output>, PreprocessingUpdatableSupervisedTemporalEstimator&lt;Preprocessor, Estimator>.Annotation>], validateOn: [AnnotatedFeature&lt;PreprocessedFeatureSequence&lt;Preprocessor.Output>, PreprocessingUpdatableSupervisedTemporalEstimator&lt;Preprocessor, Estimator>.Annotation>], eventHandler: EventHandler?) async throws -> PreprocessingUpdatableSupervisedTemporalEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a transformer to a sequence of preprocessed features while validating.

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

