

- Create ML Components
- PreprocessingTabularEstimator
-  fitted(toPreprocessed:eventHandler:) 

Instance Method

# fitted(toPreprocessed:eventHandler:)

Fits a transformer to a data frame of preprocessed features.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
func fitted(
    toPreprocessed preprocessed: DataFrame,
    eventHandler: EventHandler? = nil
) async throws -> PreprocessingTabularEstimator.Transformer
```

## Parameters 

`preprocessed`  

A data frame of preprocessed features.

`eventHandler`  

An event handler.

## Return Value

The fitted transformer.

## See Also

### Preprocesing and fitting

func preprocessed(from: DataFrame, eventHandler: EventHandler?) async throws -> DataFrame

Preprocesses a data frame of examples.

func fitted(to: DataFrame, eventHandler: EventHandler?) async throws -> PreprocessingTabularEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a composed transformer to a data frame of examples.

typealias Input

The input type.

typealias Intermediate

The intermediate type.

typealias Output

The output type.

typealias Transformer

The transformer type created by this estimator.

