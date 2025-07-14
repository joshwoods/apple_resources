

- Create ML Components
- PreprocessingUpdatableEstimator
-  PreprocessingUpdatableEstimator.Input 

Type Alias

# PreprocessingUpdatableEstimator.Input

The input type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
typealias Input = Preprocessor.Input
```

## See Also

### Preprocesing and fitting

func preprocessed&lt;S>(from: S, eventHandler: EventHandler?) async throws -> [Preprocessor.Output]

Preprocesses a sequence of examples.

func fitted&lt;S>(to: S, eventHandler: EventHandler?) async throws -> PreprocessingUpdatableEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a composed transformer to a sequence of examples.

func fitted&lt;S>(toPreprocessed: S, eventHandler: EventHandler?) async throws -> PreprocessingUpdatableEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a transformer to a sequence of preprocessed features.

func makeTransformer() -> PreprocessingUpdatableEstimator&lt;Preprocessor, Estimator>.Transformer

Creates a default-initialized transformer suitable for incremental fitting.

func update&lt;InputSequence>(inout PreprocessingUpdatableEstimator&lt;Preprocessor, Estimator>.Transformer, with: InputSequence, eventHandler: EventHandler?) async throws

Updates a transformer with a new sequence of examples.

func update&lt;InputSequence>(inout PreprocessingUpdatableEstimator&lt;Preprocessor, Estimator>.Transformer, withPreprocessed: InputSequence, eventHandler: EventHandler?) async throws

Updates a transformer with a new sequence of preprocessed features.

typealias Intermediate

The intermediate type.

typealias Output

The output type.

typealias Transformer

The transformer type created by this estimator.

