

- SwiftUI
- GraphicsContext
-  GraphicsContext.BlendMode 

Structure

# GraphicsContext.BlendMode

The ways that a graphics context combines new content with background content.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@frozen
struct BlendMode
```

## Overview

Use one of these values to set the blendMode property of a GraphicsContext. The value that you set affects how content that you draw replaces or combines with content that you previously drew into the context.

## Topics

### Getting the default

static var normal: GraphicsContext.BlendMode

A mode that paints source image samples over the background image samples.

### Darkening

static var darken: GraphicsContext.BlendMode

A mode that creates composite image samples by choosing the darker samples from either the source image or the background.

static var multiply: GraphicsContext.BlendMode

A mode that multiplies the source image samples with the background image samples.

static var colorBurn: GraphicsContext.BlendMode

A mode that darkens background image samples to reflect the source image samples.

static var plusDarker: GraphicsContext.BlendMode

A mode that adds the inverse of the color components of the source and background images, and then inverts the result, producing a darkened composite.

### Lightening

static var lighten: GraphicsContext.BlendMode

A mode that creates composite image samples by choosing the lighter samples from either the source image or the background.

static var screen: GraphicsContext.BlendMode

A mode that multiplies the inverse of the source image samples with the inverse of the background image samples.

static var colorDodge: GraphicsContext.BlendMode

A mode that brightens the background image samples to reflect the source image samples.

static var plusLighter: GraphicsContext.BlendMode

A mode that adds the components of the source and background images, resulting in a lightened composite.

### Adding contrast

static var overlay: GraphicsContext.BlendMode

A mode that either multiplies or screens the source image samples with the background image samples, depending on the background color.

static var softLight: GraphicsContext.BlendMode

A mode that either darkens or lightens colors, depending on the source image sample color.

static var hardLight: GraphicsContext.BlendMode

A mode that either multiplies or screens colors, depending on the source image sample color.

### Inverting

static var difference: GraphicsContext.BlendMode

A mode that subtracts the brighter of the source image sample color or the background image sample color from the other.

static var exclusion: GraphicsContext.BlendMode

A mode that produces an effect similar to that produced by the difference blend mode, but with lower contrast.

### Mixing color components

static var hue: GraphicsContext.BlendMode

A mode that uses the luminance and saturation values of the background with the hue of the source image.

static var saturation: GraphicsContext.BlendMode

A mode that uses the luminance and hue values of the background with the saturation of the source image.

static var color: GraphicsContext.BlendMode

A mode that uses the luminance values of the background with the hue and saturation values of the source image.

static var luminosity: GraphicsContext.BlendMode

A mode that uses the hue and saturation of the background with the luminance of the source image.

### Accessing porter-duff modes

static var clear: GraphicsContext.BlendMode

A mode that clears any pixels that the source image overwrites.

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

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Equatable
- RawRepresentable
- Sendable

## See Also

### Setting opacity and the blend mode

var opacity: Double

The opacity of drawing operations in the context.

var blendMode: GraphicsContext.BlendMode

The blend mode used by drawing operations in the context.

