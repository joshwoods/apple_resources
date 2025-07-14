

- SwiftUI
- GraphicsContext
-  clipToLayer(opacity:options:content:) 

Instance Method

# clipToLayer(opacity:options:content:)

Adds a clip shape that you define in a new layer to the context’s array of clip shapes.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
mutating func clipToLayer(
    opacity: Double = 1,
    options: GraphicsContext.ClipOptions = ClipOptions(),
    content: (inout GraphicsContext) throws -> Void
) rethrows
```

## Parameters 

`opacity`  

A value that SwiftUI uses to multiply the alpha channel of the rasterized layer that you define in the `content` closure. The alpha values that result define the clip shape.

`options`  

A set of options that tell SwiftUI how to interpret the clip shape. For example, you can invert the clip shape by setting the inverse option.

`content`  

A closure that receives as input a new GraphicsContext, which represents a new transparency layer. The alpha channel of content that you draw into this context, multiplied by the `opacity` parameter, defines the clip shape.

## Discussion

Call this method to add a shape to the array of clip shapes that the context uses to define a clipping mask. Shapes that you add affect only subsequent drawing operations.

## See Also

### Masking

func clip(to: Path, style: FillStyle, options: GraphicsContext.ClipOptions)

Adds a path to the context’s array of clip shapes.

var clipBoundingRect: CGRect

The bounding rectangle of the intersection of all current clip shapes in the current user space.

struct ClipOptions

Options that affect the use of clip shapes.

