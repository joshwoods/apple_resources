

- SwiftUI
- Shape
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
) -> _ShapeView where S : ShapeStyle
```

Show all declarations

## Parameters 

`content`  

The color or gradient to use when filling this shape.

`style`  

The style options that determine how the fill renders.

## Return Value

A shape filled with the color or gradient you supply.

## See Also

### Filling a shape

func fill(style: FillStyle) -> some View

Fills this shape with the foreground color.

