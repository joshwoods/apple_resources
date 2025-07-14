

- SwiftUI
- GraphicsContext
-  clip(to:style:options:) 

Instance Method

# clip(to:style:options:)

Adds a path to the context’s array of clip shapes.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
mutating func clip(
    to path: Path,
    style: FillStyle = FillStyle(),
    options: GraphicsContext.ClipOptions = ClipOptions()
)
```

## Parameters 

`path`  

A Path that defines the shape of the clipping mask.

`style`  

A FillStyle that defines how to rasterize the shape.

`options`  

Clip options that tell SwiftUI how to interpret the `path` as a clip shape. For example, you can invert the clip shape by setting the inverse option.

## Discussion

Call this method to add a shape to the array of clip shapes that the context uses to define a clipping mask. Shapes that you add affect only subsequent drawing operations.

## See Also

### Masking

func clipToLayer(opacity: Double, options: GraphicsContext.ClipOptions, content: (inout GraphicsContext) throws -> Void) rethrows

Adds a clip shape that you define in a new layer to the context’s array of clip shapes.

var clipBoundingRect: CGRect

The bounding rectangle of the intersection of all current clip shapes in the current user space.

struct ClipOptions

Options that affect the use of clip shapes.

