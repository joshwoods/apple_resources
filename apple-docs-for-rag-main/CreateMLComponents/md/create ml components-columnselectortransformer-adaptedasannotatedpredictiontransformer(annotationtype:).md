

- Create ML Components
- ColumnSelectorTransformer
-  adaptedAsAnnotatedPredictionTransformer(annotationType:) 

Instance Method

# adaptedAsAnnotatedPredictionTransformer(annotationType:)

Returns an annotated-prediction transformer that transforms the predictions using this transformer while leaving the annotations unchanged.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
func adaptedAsAnnotatedPredictionTransformer(annotationType: Annotation.Type = Annotation.self) -> some Transformer, AnnotatedPrediction>
```

