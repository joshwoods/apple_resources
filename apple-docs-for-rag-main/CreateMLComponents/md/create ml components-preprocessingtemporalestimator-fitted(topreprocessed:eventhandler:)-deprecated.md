

- Create ML Components
- PreprocessingTemporalEstimator
-  fitted(toPreprocessed:eventHandler:) Deprecated

Instance Method

# fitted(toPreprocessed:eventHandler:)

Fits a transformer to a sequence of preprocessed features.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func fitted(
    toPreprocessed preprocessed: [PreprocessedFeatureSequence],
    eventHandler: EventHandler? = nil
) async throws -> PreprocessingTemporalEstimator.Transformer
```

## Parameters 

`preprocessed`  

A sequence of preprocessed featuress.

`eventHandler`  

An event handler.

## Return Value

The fitted transformer.

## See Also

### Preprocesing and fitting

func preprocessed&lt;InputSequence>(from: InputSequence, eventHandler: EventHandler?) async throws -> [PreprocessedFeatureSequence&lt;Preprocessor.Output>]

Preprocesses a sequence of examples.

Deprecated

func fitted&lt;InputSequence>(to: InputSequence, eventHandler: EventHandler?) async throws -> PreprocessingTemporalEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a transformer to a sequence of examples.

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

