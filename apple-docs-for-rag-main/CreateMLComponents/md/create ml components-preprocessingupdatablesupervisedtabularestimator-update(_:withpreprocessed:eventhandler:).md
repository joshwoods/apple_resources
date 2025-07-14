

- Create ML Components
- PreprocessingUpdatableSupervisedTabularEstimator
-  update(\_:withPreprocessed:eventHandler:) 

Instance Method

# update(\_:withPreprocessed:eventHandler:)

Updates a transformer with a new data frame of preprocessed features.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
func update(
    _ transformer: inout PreprocessingUpdatableSupervisedTabularEstimator.Transformer,
    withPreprocessed preprocessed: DataFrame,
    eventHandler: EventHandler? = nil
) async throws
```

## Parameters 

`transformer`  

A transformer to update.

`preprocessed`  

A data frame of preprocessed features.

`eventHandler`  

An event handler.

## See Also

### Preprocesing and fitting

func fitted(to: DataFrame, validateOn: DataFrame?, eventHandler: EventHandler?) async throws -> PreprocessingUpdatableSupervisedTabularEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a composed transformer to a data frame of examples.

func fitted(toPreprocessed: DataFrame, validateOn: DataFrame?, eventHandler: EventHandler?) async throws -> PreprocessingUpdatableSupervisedTabularEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a composed transformer to a data frame of examples.

func makeTransformer() -> PreprocessingUpdatableSupervisedTabularEstimator&lt;Preprocessor, Estimator>.Transformer

Creates a default-initialized transformer suitable for incremental fitting.

func preprocessed(from: DataFrame, eventHandler: EventHandler?) async throws -> DataFrame

Preprocesses a data frame.

func update(inout PreprocessingUpdatableSupervisedTabularEstimator&lt;Preprocessor, Estimator>.Transformer, with: DataFrame, eventHandler: EventHandler?) async throws

Updates a transformer with a new data frame of examples.

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

