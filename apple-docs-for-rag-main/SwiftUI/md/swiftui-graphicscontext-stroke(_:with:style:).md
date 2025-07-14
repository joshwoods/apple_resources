

- SwiftUI
- GraphicsContext
-  stroke(\_:with:style:) 

Instance Method

# stroke(\_:with:style:)

Draws a path into the context with a specified stroke style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func stroke(
    _ path: Path,
    with shading: GraphicsContext.Shading,
    style: StrokeStyle
)
```

## Parameters 

`path`  

The path to outline.

`shading`  

The color or pattern to use when outlining the `path`.

`style`  

A style that indicates how to outline the path.

## Discussion

If you only need to control the style’s lineWidth property, use stroke(_:with:lineWidth:) instead.

## See Also

### Drawing a path

func stroke(Path, with: GraphicsContext.Shading, lineWidth: CGFloat)

Draws a path into the context with a specified line width.

func fill(Path, with: GraphicsContext.Shading, style: FillStyle)

Draws a path into the context and fills the outlined region.

struct Shading

A color or pattern that you can use to outline or fill a path.

struct GradientOptions

Options that affect the rendering of color gradients.

