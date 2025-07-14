

- SwiftUI
- Shape
-  stroke(style:) 

Instance Method

# stroke(style:)

Returns a new shape that is a stroked copy of `self`, using the contents of `style` to define the stroke characteristics.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
func stroke(style: StrokeStyle) -> some Shape
```

## See Also

### Setting the stroke characteristics

func stroke&lt;S>(S, lineWidth: CGFloat) -> some View

Traces the outline of this shape with a color or gradient.

func stroke&lt;S>(S, lineWidth: CGFloat, antialiased: Bool) -> StrokeShapeView&lt;Self, S, EmptyView>

Traces the outline of this shape with a color or gradient.

func stroke(lineWidth: CGFloat) -> some Shape

Returns a new shape that is a stroked copy of `self` with line-width defined by `lineWidth` and all other properties of `StrokeStyle` having their default values.

func stroke&lt;S>(S, style: StrokeStyle) -> some View

Traces the outline of this shape with a color or gradient.

func stroke&lt;S>(S, style: StrokeStyle, antialiased: Bool) -> StrokeShapeView&lt;Self, S, EmptyView>

Traces the outline of this shape with a color or gradient.

