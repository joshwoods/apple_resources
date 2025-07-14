

- Create ML Components
- PreprocessingSupervisedTabularEstimator
-  fitted(toPreprocessed:validateOn:eventHandler:) 

Instance Method

# fitted(toPreprocessed:validateOn:eventHandler:)

Fits a transformer to a data frame of preprocessed examples while validating.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
func fitted(
    toPreprocessed preprocessedInput: DataFrame,
    validateOn preprocessedValidation: DataFrame?,
    eventHandler: EventHandler? = nil
) async throws -> PreprocessingSupervisedTabularEstimator.Transformer
```

## Parameters 

`preprocessedInput`  

A data frame of preprocessed features used for fitting the transformer.

`preprocessedValidation`  

A data frame of preprocessed features used for validating the fitted transformer.

`eventHandler`  

An event handler.

## Return Value

The fitted transformer.

## See Also

### Preprocesing and fitting

func preprocessed(from: DataFrame, eventHandler: EventHandler?) async throws -> DataFrame

Preprocesses a data frame of examples.

func fitted(to: DataFrame, validateOn: DataFrame?, eventHandler: EventHandler?) async throws -> PreprocessingSupervisedTabularEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a transformer to a data frame

typealias Annotation

The annotation type.

typealias Input

The input type.

typealias Intermediate

The intermediate type.

typealias Output

The output type.

typealias Transformer

The transformer type created by this estimator.

