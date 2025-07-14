

- Create ML Components
- ImageReader
-  adaptedAsAnnotatedFeatureTransformer(annotationType:) 

Instance Method

# adaptedAsAnnotatedFeatureTransformer(annotationType:)

Returns an annotated-feature transformer that transforms the features using this transformer while leaving the annotations unchanged.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
func adaptedAsAnnotatedFeatureTransformer(annotationType: Annotation.Type = Annotation.self) -> some Transformer, AnnotatedFeature>
```

