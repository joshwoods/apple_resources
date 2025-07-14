

- SwiftUI
- GraphicsContext
- GraphicsContext.BlendMode
-  clear 

Type Property

# clear

A mode that clears any pixels that the source image overwrites.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var clear: GraphicsContext.BlendMode { get }
```

## Discussion

With this mode, you can use the source image like an eraser.

This mode implements the equation `R = 0` where `R` is the composite image.

## See Also

### Accessing porter-duff modes

static var copy: GraphicsContext.BlendMode

A mode that replaces background image samples with source image samples.

static var sourceIn: GraphicsContext.BlendMode

A mode that you use to paint the source image, including its transparency, onto the opaque parts of the background.

static var sourceOut: GraphicsContext.BlendMode

A mode that you use to paint the source image onto the transparent parts of the background, while erasing the background.

static var sourceAtop: GraphicsContext.BlendMode

A mode that you use to paint the opaque parts of the source image onto the opaque parts of the background.

static var destinationOver: GraphicsContext.BlendMode

A mode that you use to paint the source image under the background.

static var destinationIn: GraphicsContext.BlendMode

A mode that you use to erase any of the background that isn’t covered by opaque source pixels.

static var destinationOut: GraphicsContext.BlendMode

A mode that you use to erase any of the background that is covered by opaque source pixels.

static var destinationAtop: GraphicsContext.BlendMode

A mode that you use to paint the source image under the background, while erasing any of the background not matched by opaque pixels from the source image.

static var xor: GraphicsContext.BlendMode

A mode that you use to clear pixels where both the source and background images are opaque.

