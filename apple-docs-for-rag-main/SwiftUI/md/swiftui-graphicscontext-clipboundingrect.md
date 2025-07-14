

- SwiftUI
- GraphicsContext
-  clipBoundingRect 

Instance Property

# clipBoundingRect

The bounding rectangle of the intersection of all current clip shapes in the current user space.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var clipBoundingRect: CGRect { get }
```

## See Also

### Masking

func clip(to: Path, style: FillStyle, options: GraphicsContext.ClipOptions)

Adds a path to the context’s array of clip shapes.

func clipToLayer(opacity: Double, options: GraphicsContext.ClipOptions, content: (inout GraphicsContext) throws -> Void) rethrows

Adds a clip shape that you define in a new layer to the context’s array of clip shapes.

struct ClipOptions

Options that affect the use of clip shapes.

