

- SwiftUI
- ShapeView
-  fill(\_:style:) 

Instance Method

# fill(\_:style:)

Fills this shape with a color or gradient.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
func fill(
    _ content: S = .foreground,
    style: FillStyle = FillStyle()
) -> FillShapeView where S : ShapeStyle
```

## Parameters 

`content`  

The color or gradient to use when filling this shape.

`style`  

The style options that determine how the fill renders.

## Return Value

A shape filled with the color or gradient you supply.

## See Also

### Modify the shape

func stroke&lt;S>(S, style: StrokeStyle, antialiased: Bool) -> StrokeShapeView&lt;Self.Content, S, Self>

Traces the outline of this shape with a color or gradient.

func stroke&lt;S>(S, lineWidth: CGFloat, antialiased: Bool) -> StrokeShapeView&lt;Self.Content, S, Self>

Traces the outline of this shape with a color or gradient.

func strokeBorder&lt;S>(S, style: StrokeStyle, antialiased: Bool) -> StrokeBorderShapeView&lt;Self.Content, S, Self>

Returns a view that’s the result of insetting this view by half of its style’s line width.

func strokeBorder&lt;S>(S, lineWidth: CGFloat, antialiased: Bool) -> StrokeBorderShapeView&lt;Self.Content, S, Self>

Returns a view that’s the result of filling an inner stroke of this view with the content you supply.

