

- Create ML Components
- PreprocessingTabularEstimator
-  PreprocessingTabularEstimator.Transformer 

Type Alias

# PreprocessingTabularEstimator.Transformer

The transformer type created by this estimator.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
typealias Transformer = ComposedTabularTransformer
```

## See Also

### Preprocesing and fitting

func preprocessed(from: DataFrame, eventHandler: EventHandler?) async throws -> DataFrame

Preprocesses a data frame of examples.

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

