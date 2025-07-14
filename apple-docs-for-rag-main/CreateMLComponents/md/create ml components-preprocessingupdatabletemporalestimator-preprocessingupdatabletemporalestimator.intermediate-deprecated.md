

- Create ML Components
- PreprocessingUpdatableTemporalEstimator
-  PreprocessingUpdatableTemporalEstimator.Intermediate Deprecated

Type Alias

# PreprocessingUpdatableTemporalEstimator.Intermediate

The intermediate type.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
typealias Intermediate = Preprocessor.Output
```

## See Also

### Preprocesing and fitting

func preprocessed&lt;InputSequence>(from: InputSequence, eventHandler: EventHandler?) async throws -> [PreprocessedFeatureSequence&lt;Preprocessor.Output>]

Preprocesses a sequence of examples.

Deprecated

func fitted&lt;InputSequence>(to: InputSequence, eventHandler: EventHandler?) async throws -> PreprocessingUpdatableTemporalEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a transformer to a sequence of examples.

Deprecated

func fitted(toPreprocessed: [PreprocessedFeatureSequence&lt;Preprocessor.Output>], eventHandler: EventHandler?) async throws -> PreprocessingUpdatableTemporalEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a transformer to a sequence of preprocessed features.

Deprecated

func update&lt;InputSequence>(inout PreprocessingUpdatableTemporalEstimator&lt;Preprocessor, Estimator>.Transformer, withPreprocessed: InputSequence, eventHandler: EventHandler?) async throws

Updates a transformer with a new sequence of preprocessed features.

Deprecated

func update&lt;InputSequence>(inout PreprocessingUpdatableTemporalEstimator&lt;Preprocessor, Estimator>.Transformer, with: InputSequence, eventHandler: EventHandler?) async throws

Updates a transformer with a new sequence of examples.

Deprecated

func makeTransformer() -> PreprocessingUpdatableTemporalEstimator&lt;Preprocessor, Estimator>.Transformer

Creates a default-initialized transformer suitable for incremental fitting.

Deprecated

typealias Input

The input type.

Deprecated

typealias Output

The output type.

Deprecated

typealias Transformer

The transformer type created by this estimator.

Deprecated

