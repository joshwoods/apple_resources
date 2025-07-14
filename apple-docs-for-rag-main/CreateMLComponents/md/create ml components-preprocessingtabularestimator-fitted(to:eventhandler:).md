

- Create ML Components
- PreprocessingTabularEstimator
-  fitted(to:eventHandler:) 

Instance Method

# fitted(to:eventHandler:)

Fits a composed transformer to a data frame of examples.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
func fitted(
    to input: DataFrame,
    eventHandler: EventHandler? = nil
) async throws -> PreprocessingTabularEstimator.Transformer
```

## Parameters 

`input`  

A data frame of examples.

`eventHandler`  

An event handler.

## Return Value

The fitted transformer.

## See Also

### Preprocesing and fitting

func preprocessed(from: DataFrame, eventHandler: EventHandler?) async throws -> DataFrame

Preprocesses a data frame of examples.

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

