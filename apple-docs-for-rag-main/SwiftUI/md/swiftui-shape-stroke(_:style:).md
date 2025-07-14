

- SwiftUI
- Shape
-  stroke(\_:style:) 

Instance Method

# stroke(\_:style:)

Traces the outline of this shape with a color or gradient.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
func stroke(
    _ content: S,
    style: StrokeStyle
) -> some View where S : ShapeStyle
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

### Setting the stroke characteristics

func stroke&lt;S>(S, lineWidth: CGFloat) -> some View

Traces the outline of this shape with a color or gradient.

func stroke&lt;S>(S, lineWidth: CGFloat, antialiased: Bool) -> StrokeShapeView&lt;Self, S, EmptyView>

Traces the outline of this shape with a color or gradient.

func stroke(lineWidth: CGFloat) -> some Shape

Returns a new shape that is a stroked copy of `self` with line-width defined by `lineWidth` and all other properties of `StrokeStyle` having their default values.

func stroke&lt;S>(S, style: StrokeStyle, antialiased: Bool) -> StrokeShapeView&lt;Self, S, EmptyView>

Traces the outline of this shape with a color or gradient.

func stroke(style: StrokeStyle) -> some Shape

Returns a new shape that is a stroked copy of `self`, using the contents of `style` to define the stroke characteristics.

