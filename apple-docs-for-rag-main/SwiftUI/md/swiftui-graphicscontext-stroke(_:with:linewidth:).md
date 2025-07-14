

- SwiftUI
- GraphicsContext
-  stroke(\_:with:lineWidth:) 

Instance Method

# stroke(\_:with:lineWidth:)

Draws a path into the context with a specified line width.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func stroke(
    _ path: Path,
    with shading: GraphicsContext.Shading,
    lineWidth: CGFloat = 1
)
```

## Parameters 

`path`  

The path to outline.

`shading`  

The color or pattern to use when outlining the `path`.

`lineWidth`  

The width of the stroke, which defaults to `1`.

## Discussion

When you call this method, all StrokeStyle properties other than lineWidth take their default values. To control other style properties, use stroke(_:with:style:) instead.

## See Also

### Drawing a path

func stroke(Path, with: GraphicsContext.Shading, style: StrokeStyle)

Draws a path into the context with a specified stroke style.

func fill(Path, with: GraphicsContext.Shading, style: FillStyle)

Draws a path into the context and fills the outlined region.

struct Shading

A color or pattern that you can use to outline or fill a path.

struct GradientOptions

Options that affect the rendering of color gradients.

