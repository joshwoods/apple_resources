

- SwiftUI
- Shape
-  stroke(\_:lineWidth:antialiased:) 

Instance Method

# stroke(\_:lineWidth:antialiased:)

Traces the outline of this shape with a color or gradient.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
func stroke(
    _ content: S,
    lineWidth: CGFloat = 1,
    antialiased: Bool = true
) -> StrokeShapeView where S : ShapeStyle
```

## Parameters 

`content`  

The color or gradient with which to stroke this shape.

`lineWidth`  

The width of the stroke that outlines this shape.

## Return Value

A stroked shape.

## Discussion

The following example draws a circle with a purple stroke:

```
Circle().stroke(Color.purple, lineWidth: 5)
```

## See Also

### Setting the stroke characteristics

func stroke&lt;S>(S, lineWidth: CGFloat) -> some View

Traces the outline of this shape with a color or gradient.

func stroke(lineWidth: CGFloat) -> some Shape

Returns a new shape that is a stroked copy of `self` with line-width defined by `lineWidth` and all other properties of `StrokeStyle` having their default values.

func stroke&lt;S>(S, style: StrokeStyle) -> some View

Traces the outline of this shape with a color or gradient.

func stroke&lt;S>(S, style: StrokeStyle, antialiased: Bool) -> StrokeShapeView&lt;Self, S, EmptyView>

Traces the outline of this shape with a color or gradient.

func stroke(style: StrokeStyle) -> some Shape

Returns a new shape that is a stroked copy of `self`, using the contents of `style` to define the stroke characteristics.

