

- SwiftUI
- ShapeView
-  strokeBorder(\_:style:antialiased:) 

Instance Method

# strokeBorder(\_:style:antialiased:)

Returns a view that’s the result of insetting this view by half of its style’s line width.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
func strokeBorder(
    _ content: S = .foreground,
    style: StrokeStyle,
    antialiased: Bool = true
) -> StrokeBorderShapeView where S : ShapeStyle
```

Available when `Content` conforms to `InsettableShape`.

## Discussion

This method strokes the resulting shape with `style` and fills it with `content`.

## See Also

### Modify the shape

func fill&lt;S>(S, style: FillStyle) -> FillShapeView&lt;Self.Content, S, Self>

Fills this shape with a color or gradient.

func stroke&lt;S>(S, style: StrokeStyle, antialiased: Bool) -> StrokeShapeView&lt;Self.Content, S, Self>

Traces the outline of this shape with a color or gradient.

func stroke&lt;S>(S, lineWidth: CGFloat, antialiased: Bool) -> StrokeShapeView&lt;Self.Content, S, Self>

Traces the outline of this shape with a color or gradient.

func strokeBorder&lt;S>(S, lineWidth: CGFloat, antialiased: Bool) -> StrokeBorderShapeView&lt;Self.Content, S, Self>

Returns a view that’s the result of filling an inner stroke of this view with the content you supply.

