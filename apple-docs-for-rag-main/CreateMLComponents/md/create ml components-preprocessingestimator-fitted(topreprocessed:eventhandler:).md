

- Create ML Components
- PreprocessingEstimator
-  fitted(toPreprocessed:eventHandler:) 

Instance Method

# fitted(toPreprocessed:eventHandler:)

Fits a transformer to a sequence of preprocessed features.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func fitted(
    toPreprocessed preprocessed: S,
    eventHandler: EventHandler? = nil
) async throws -> PreprocessingEstimator.Transformer where S : Sequence, Preprocessor.Output == S.Element, S.Element == Estimator.Transformer.Input
```

## Parameters 

`preprocessed`  

A sequence of preprocessed features.

`eventHandler`  

An event handler.

## Return Value

The fitted transformer.

## See Also

### Preprocesing and fitting

func preprocessed&lt;S>(from: S, eventHandler: EventHandler?) async throws -> [Preprocessor.Output]

Preprocesses a sequence of examples.

func fitted&lt;S>(to: S, eventHandler: EventHandler?) async throws -> PreprocessingEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a composed transformer to a sequence of examples.

typealias Input

The input type.

typealias Intermediate

The intermediate type.

typealias Output

The output type.

typealias Transformer

The transformer type created by this estimator.

