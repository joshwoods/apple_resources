

- SwiftUI
- ShapeView
-  stroke(\_:style:antialiased:) 

Instance Method

# stroke(\_:style:antialiased:)

Traces the outline of this shape with a color or gradient.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
func stroke(
    _ content: S,
    style: StrokeStyle,
    antialiased: Bool = true
) -> StrokeShapeView where S : ShapeStyle
```

## Parameters 

`content`  

The color or gradient with which to stroke this shape.

`style`  

The stroke characteristics — such as the line’s width and whether the stroke is dashed — that determine how to render this shape.

## Return Value

A stroked shape.

## Discussion

The following example adds a dashed purple stroke to a `Capsule`:

```
Capsule()
.stroke(
    Color.purple,
    style: StrokeStyle(
        lineWidth: 5,
        lineCap: .round,
        lineJoin: .miter,
        miterLimit: 0,
        dash: [5, 10],
        dashPhase: 0
    )
)
```

## See Also

### Modify the shape

func fill&lt;S>(S, style: FillStyle) -> FillShapeView&lt;Self.Content, S, Self>

Fills this shape with a color or gradient.

func stroke&lt;S>(S, lineWidth: CGFloat, antialiased: Bool) -> StrokeShapeView&lt;Self.Content, S, Self>

Traces the outline of this shape with a color or gradient.

func strokeBorder&lt;S>(S, style: StrokeStyle, antialiased: Bool) -> StrokeBorderShapeView&lt;Self.Content, S, Self>

Returns a view that’s the result of insetting this view by half of its style’s line width.

func strokeBorder&lt;S>(S, lineWidth: CGFloat, antialiased: Bool) -> StrokeBorderShapeView&lt;Self.Content, S, Self>

Returns a view that’s the result of filling an inner stroke of this view with the content you supply.

