

- Create ML Components
- PreprocessingUpdatableTemporalEstimator
-  update(\_:withPreprocessed:eventHandler:) Deprecated

Instance Method

# update(\_:withPreprocessed:eventHandler:)

Updates a transformer with a new sequence of preprocessed features.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func update(
    _ transformer: inout PreprocessingUpdatableTemporalEstimator.Transformer,
    withPreprocessed preprocessed: InputSequence,
    eventHandler: EventHandler? = nil
) async throws where InputSequence : Sequence, InputSequence.Element : TemporalSequence, Estimator.Transformer.Input == InputSequence.Element.Feature
```

## Parameters 

`transformer`  

A transformer to update.

`preprocessed`  

A sequence of preprocessed features.

`eventHandler`  

An event handler.

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

func update&lt;InputSequence>(inout PreprocessingUpdatableTemporalEstimator&lt;Preprocessor, Estimator>.Transformer, with: InputSequence, eventHandler: EventHandler?) async throws

Updates a transformer with a new sequence of examples.

Deprecated

func makeTransformer() -> PreprocessingUpdatableTemporalEstimator&lt;Preprocessor, Estimator>.Transformer

Creates a default-initialized transformer suitable for incremental fitting.

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

