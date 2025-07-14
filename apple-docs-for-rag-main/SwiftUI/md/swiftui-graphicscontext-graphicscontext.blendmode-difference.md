

- SwiftUI
- GraphicsContext
- GraphicsContext.BlendMode
-  difference 

Type Property

# difference

A mode that subtracts the brighter of the source image sample color or the background image sample color from the other.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var difference: GraphicsContext.BlendMode { get }
```

## Discussion

Source image sample values that are black produce no change; white inverts the background color values.

## See Also

### Inverting

static var exclusion: GraphicsContext.BlendMode

A mode that produces an effect similar to that produced by the difference blend mode, but with lower contrast.

