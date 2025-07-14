

- Create ML Components
- PreprocessingSupervisedTabularEstimator
-  PreprocessingSupervisedTabularEstimator.Input 

Type Alias

# PreprocessingSupervisedTabularEstimator.Input

The input type.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
typealias Input = Preprocessor.Input
```

## See Also

### Preprocesing and fitting

func preprocessed(from: DataFrame, eventHandler: EventHandler?) async throws -> DataFrame

Preprocesses a data frame of examples.

func fitted(to: DataFrame, validateOn: DataFrame?, eventHandler: EventHandler?) async throws -> PreprocessingSupervisedTabularEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a transformer to a data frame

func fitted(toPreprocessed: DataFrame, validateOn: DataFrame?, eventHandler: EventHandler?) async throws -> PreprocessingSupervisedTabularEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a transformer to a data frame of preprocessed examples while validating.

typealias Annotation

The annotation type.

typealias Intermediate

The intermediate type.

typealias Output

The output type.

typealias Transformer

The transformer type created by this estimator.

