

- Create ML Components
- Transformer
-  Input 

Associated Type

# Input

The input type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
associatedtype Input
```

**Required**

## See Also

### Applying and adapting

func applied(to: Self.Input, eventHandler: EventHandler?) async throws -> Self.Output

Performs the transformation on a single input.

**Required** Default implementations provided.

func adaptedAsAnnotatedFeatureTransformer&lt;Annotation>(annotationType: Annotation.Type) -> some Transformer&lt;AnnotatedFeature&lt;Self.Input, Annotation>, AnnotatedFeature&lt;Self.Output, Annotation>> 

Returns an annotated-feature transformer that transforms the features using this transformer while leaving the annotations unchanged.

func adaptedAsAnnotatedPredictionTransformer&lt;Annotation>(annotationType: Annotation.Type) -> some Transformer&lt;AnnotatedPrediction&lt;Self.Input, Annotation>, AnnotatedPrediction&lt;Self.Output, Annotation>> 

Returns an annotated-prediction transformer that transforms the predictions using this transformer while leaving the annotations unchanged.

func adaptedAsEstimator() -> TransformerToEstimatorAdaptor&lt;Self>

Exposes this transformer as a trivial estimator.

func adaptedAsRandomTransformer() -> some RandomTransformer&lt;Self.Input, Self.Output> 

Returns a random transformer wrapping a transformer.

func adaptedAsUpdatableEstimator() -> TransformerToUpdatableEstimatorAdaptor&lt;Self>

Exposes this transformer as a trivial estimator.

associatedtype Output

The output type.

**Required**

