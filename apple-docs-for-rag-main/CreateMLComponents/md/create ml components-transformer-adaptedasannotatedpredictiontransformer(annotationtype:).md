

- Create ML Components
- Transformer
-  adaptedAsAnnotatedPredictionTransformer(annotationType:) 

Instance Method

# adaptedAsAnnotatedPredictionTransformer(annotationType:)

Returns an annotated-prediction transformer that transforms the predictions using this transformer while leaving the annotations unchanged.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
func adaptedAsAnnotatedPredictionTransformer(annotationType: Annotation.Type = Annotation.self) -> some Transformer, AnnotatedPrediction>
```

## See Also

### Applying and adapting

func applied(to: Self.Input, eventHandler: EventHandler?) async throws -> Self.Output

Performs the transformation on a single input.

**Required** Default implementations provided.

func adaptedAsAnnotatedFeatureTransformer&lt;Annotation>(annotationType: Annotation.Type) -> some Transformer&lt;AnnotatedFeature&lt;Self.Input, Annotation>, AnnotatedFeature&lt;Self.Output, Annotation>> 

Returns an annotated-feature transformer that transforms the features using this transformer while leaving the annotations unchanged.

func adaptedAsEstimator() -> TransformerToEstimatorAdaptor&lt;Self>

Exposes this transformer as a trivial estimator.

func adaptedAsRandomTransformer() -> some RandomTransformer&lt;Self.Input, Self.Output> 

Returns a random transformer wrapping a transformer.

func adaptedAsUpdatableEstimator() -> TransformerToUpdatableEstimatorAdaptor&lt;Self>

Exposes this transformer as a trivial estimator.

associatedtype Input

The input type.

**Required**

associatedtype Output

The output type.

**Required**

