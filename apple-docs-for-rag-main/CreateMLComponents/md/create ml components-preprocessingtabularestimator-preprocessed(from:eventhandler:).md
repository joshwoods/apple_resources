

- Create ML Components
- PreprocessingTabularEstimator
-  preprocessed(from:eventHandler:) 

Instance Method

# preprocessed(from:eventHandler:)

Preprocesses a data frame of examples.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
func preprocessed(
    from input: DataFrame,
    eventHandler: EventHandler? = nil
) async throws -> DataFrame
```

## Parameters 

`input`  

A data frame of examples.

`eventHandler`  

An event handler.

## Return Value

The preprocessed examples.

## See Also

### Preprocesing and fitting

func fitted(to: DataFrame, eventHandler: EventHandler?) async throws -> PreprocessingTabularEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a composed transformer to a data frame of examples.

func fitted(toPreprocessed: DataFrame, eventHandler: EventHandler?) async throws -> PreprocessingTabularEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a transformer to a data frame of preprocessed features.

typealias Input

The input type.

typealias Intermediate

The intermediate type.

typealias Output

The output type.

typealias Transformer

The transformer type created by this estimator.

