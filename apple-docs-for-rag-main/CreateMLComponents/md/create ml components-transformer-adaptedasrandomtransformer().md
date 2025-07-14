

- Create ML Components
- Transformer
-  adaptedAsRandomTransformer() 

Instance Method

# adaptedAsRandomTransformer()

Returns a random transformer wrapping a transformer.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
func adaptedAsRandomTransformer() -> some RandomTransformer
```

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

func adaptedAsUpdatableEstimator() -> TransformerToUpdatableEstimatorAdaptor&lt;Self>

Exposes this transformer as a trivial estimator.

associatedtype Input

The input type.

**Required**

associatedtype Output

The output type.

**Required**

