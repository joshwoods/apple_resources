

- Create ML Components
- PreprocessingSupervisedEstimator
-  PreprocessingSupervisedEstimator.Output 

Type Alias

# PreprocessingSupervisedEstimator.Output

The output type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
typealias Output = Estimator.Transformer.Output
```

## See Also

### Preprocessing and fitting

func preprocessed&lt;S>(from: S, eventHandler: EventHandler?) async throws -> AnySequence&lt;AnnotatedFeature&lt;Preprocessor.Output, PreprocessingSupervisedEstimator&lt;Preprocessor, Estimator>.Annotation>>

Preprocesses a sequence of examples.

func fitted&lt;InputSequence>(to: InputSequence, eventHandler: EventHandler?) async throws -> PreprocessingSupervisedEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a composed transformer to a sequence of examples.

func fitted&lt;S>(toPreprocessed: S, eventHandler: EventHandler?) async throws -> PreprocessingSupervisedEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a transformer to a sequence of preprocessed features.

func fitted&lt;InputSequence, Validation>(to: InputSequence, validateOn: Validation, eventHandler: EventHandler?) async throws -> PreprocessingSupervisedEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a composed transformer to a sequence of examples.

func fitted&lt;Input, Validation>(toPreprocessed: Input, validateOn: Validation, eventHandler: EventHandler?) async throws -> PreprocessingSupervisedEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a composed transformer to a sequence of preprocessed features.

typealias Annotation

The annotation type.

typealias Input

The input type.

typealias Intermediate

The intermediate type.

typealias Transformer

The transformer type created by this estimator.

