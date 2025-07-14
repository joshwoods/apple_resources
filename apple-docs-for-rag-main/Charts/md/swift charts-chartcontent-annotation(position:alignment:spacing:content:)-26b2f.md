

- Swift Charts
- ChartContent
-  annotation(position:alignment:spacing:content:) 

Instance Method

# annotation(position:alignment:spacing:content:)

Annotates this mark or collection of marks with a view positioned relative to its bounds.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func annotation(
    position: AnnotationPosition = .automatic,
    alignment: Alignment = .center,
    spacing: CGFloat? = nil,
    @ViewBuilder content: @escaping (AnnotationContext) -> C
) -> some ChartContent where C : View
```

## Parameters 

`position`  

The location relative to the item being annotated at which the annotation will be placed.

`alignment`  

The guide for aligning the annotation in the specified position.

`spacing`  

Distance between the annotation and the annotated content, or `nil` if you want to use the default distance.

`content`  

A view builder that creates the annotation.

## See Also

### Annotating marks

func annotation&lt;C>(position: AnnotationPosition, alignment: Alignment, spacing: CGFloat?, content: () -> C) -> some ChartContent

Annotates this mark or collection of marks with a view positioned relative to its bounds.

