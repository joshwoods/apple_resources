

- Create ML Components
- PreprocessingUpdatableTabularEstimator
-  fitted(to:eventHandler:) 

Instance Method

# fitted(to:eventHandler:)

Fits a composed transformer to a data frame of examples.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
func fitted(
    to input: DataFrame,
    eventHandler: EventHandler? = nil
) async throws -> PreprocessingUpdatableTabularEstimator.Transformer
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

func fitted(toPreprocessed: DataFrame, eventHandler: EventHandler?) async throws -> PreprocessingUpdatableTabularEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a transformer to a data frame of preprocessed features.

func update(inout PreprocessingUpdatableTabularEstimator&lt;Preprocessor, Estimator>.Transformer, with: DataFrame, eventHandler: EventHandler?) async throws

Updates a transformer with a new data frame of examples.

func update(inout PreprocessingUpdatableTabularEstimator&lt;Preprocessor, Estimator>.Transformer, withPreprocessed: DataFrame, eventHandler: EventHandler?) async throws

Updates a transformer with a new data frame of preprocessed features.

func makeTransformer() -> PreprocessingUpdatableTabularEstimator&lt;Preprocessor, Estimator>.Transformer

Creates a default-initialized transformer suitable for incremental fitting.

typealias Input

The input type.

typealias Intermediate

The intermediate type.

typealias Output

The output type.

typealias Transformer

The transformer type created by this estimator.

