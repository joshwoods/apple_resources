

- Core Graphics
-  CGBlendMode 

Enumeration

# CGBlendMode

Compositing operations for images.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum CGBlendMode
```

## Overview

These blend mode constants represent the Porter-Duff blend modes. The symbols in the equations for these blend modes are:

- R is the premultiplied result

- S is the source color, and includes alpha

- D is the destination color, and includes alpha

- Ra, Sa, and Da are the alpha components of R, S, and D

You can find more information on blend modes, including examples of images produced using them, and many mathematical descriptions of the modes, in *PDF Reference, Fourth Edition*, Version 1.5, Adobe Systems, Inc. If you are a former QuickDraw developer, it may be helpful for you to think of blend modes as an alternative to transfer modes

For examples of using blend modes see “Setting Blend Modes” and “Using Blend Modes With Images” in Quartz 2D Programming Guide.

## Topics

### Constants

case normal

Paints the source image samples over the background image samples.

case multiply

Multiplies the source image samples with the background image samples. This results in colors that are at least as dark as either of the two contributing sample colors.

case screen

Multiplies the inverse of the source image samples with the inverse of the background image samples, resulting in colors that are at least as light as either of the two contributing sample colors.

case overlay

case darken

case lighten

case colorDodge

Brightens the background image samples to reflect the source image samples. Source image sample values that specify black do not produce a change.

case colorBurn

Darkens the background image samples to reflect the source image samples. Source image sample values that specify white do not produce a change.

case softLight

case hardLight

case difference

case exclusion

Produces an effect similar to that produced by CGBlendMode.difference, but with lower contrast. Source image sample values that are black don’t produce a change; white inverts the background color values.

case hue

Uses the luminance and saturation values of the background with the hue of the source image.

case saturation

Uses the luminance and hue values of the background with the saturation of the source image. Areas of the background that have no saturation (that is, pure gray areas) don’t produce a change.

case color

Uses the luminance values of the background with the hue and saturation values of the source image. This mode preserves the gray levels in the image. You can use this mode to color monochrome images or to tint color images.

case luminosity

Uses the hue and saturation of the background with the luminance of the source image. This mode creates an effect that is inverse to the effect created by CGBlendMode.color.

case clear

`R = 0`

case copy

`R = S`

case sourceIn

`R = S*Da`

case sourceOut

`R = S*(1 - Da)`

case sourceAtop

`R = S*Da + D*(1 - Sa)`

case destinationOver

`R = S*(1 - Da) + D`

case destinationIn

`R = D*Sa`

case destinationOut

`R = D*(1 - Sa)`

case destinationAtop

`R = S*(1 - Da) + D*Sa`

case xor

`R = S*(1 - Da) + D*(1 - Sa)`. This XOR mode is only nominally related to the classical bitmap XOR operation, which is not supported by Core Graphics

case plusDarker

`R = MAX(0, 1 - ((1 - D) + (1 - S)))`

case plusLighter

`R = MIN(1, S + D)`

### Initializers

init?(rawValue: Int32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing a Graphics Context

func flush()

Forces all pending drawing operations in a window context to be rendered immediately to the destination device.

func synchronize()

Marks a window context for update.

func setBlendMode(CGBlendMode)

Sets how sample values are composited by a graphics context.

func setRenderingIntent(CGColorRenderingIntent)

Sets the rendering intent in the current graphics state.

