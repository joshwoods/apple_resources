

- Create ML Components
- PreprocessingEstimator
-  preprocessed(from:eventHandler:) 

Instance Method

# preprocessed(from:eventHandler:)

Preprocesses a sequence of examples.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func preprocessed(
    from input: S,
    eventHandler: EventHandler? = nil
) async throws -> [Preprocessor.Output] where S : Sequence, Preprocessor.Input == S.Element
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

func fitted&lt;S>(to: S, eventHandler: EventHandler?) async throws -> PreprocessingEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a composed transformer to a sequence of examples.

func fitted&lt;S>(toPreprocessed: S, eventHandler: EventHandler?) async throws -> PreprocessingEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a transformer to a sequence of preprocessed features.

typealias Input

The input type.

typealias Intermediate

The intermediate type.

typealias Output

The output type.

typealias Transformer

The transformer type created by this estimator.

