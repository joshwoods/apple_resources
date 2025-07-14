

- AppKit
-  NSCompositingOperation 

Enumeration

# NSCompositingOperation

Constants that describe compositing operators in terms of source and destination images, each having an opaque and transparent region.

macOS

``` source
enum NSCompositingOperation
```

## Overview

The type of operation, the source image, and the destination image determine the final output.

These compositing operators are defined in and used by compositeToPoint:fromRect:operation:, compositeToPoint:operation:, compositeToPoint:fromRect:operation:fraction:, compositeToPoint:operation:fraction:, draw(at:from:operation:fraction:), and draw(in:from:operation:fraction:). They are also used by drawing methods in other classes that take a compositing operator.

The equations after each constant represent the mathematical formulas for calculating the color value of the resulting pixel. The table below lists the meaning of each placeholder value in the equations.

| Placeholder | Meaning                                   |
|-------------|-------------------------------------------|
| `R`         | The premultiplied result color.           |
| `S`         | The source color.                         |
| `D`         | The destination color.                    |
| `Sa`        | The alpha value of the source color.      |
| `Da`        | The alpha value of the destination color. |

## Topics

### Operations for Compositing

case clear

Transparency everywhere.

case copy

The source image.

case sourceOver

The source image wherever it is opaque, and the destination image elsewhere.

case sourceIn

The source image wherever both images are opaque, and transparent elsewhere.

case sourceOut

The source image wherever it is opaque and the destination image is transparent, and transparent elsewhere.

case sourceAtop

The source image wherever both images are opaque, the destination image wherever it is opaque but the source image is transparent, and transparent elsewhere

case destinationOver

The destination image wherever it is opaque, and the source image elsewhere.

case destinationIn

The destination image wherever both images are opaque, and transparent elsewhere.

case destinationOut

The destination image wherever it is opaque and the source image is transparent, and transparent elsewhere.

case destinationAtop

The destination image wherever both images are opaque, the source image wherever it is opaque and the destination image is transparent, and transparent elsehwere.

case xor

Exclusive OR of the source and destination images.

case plusDarker

The sum of the source and destination images, with color values approach 0 as a limit.

case plusLighter

The sum of the source and destination images, with color values approach 1 as a limit.

case multiply

The source color is multiplied by the destination color.

case screen

Multiplies the complement of the destination and source color values, and then complements the result.

case overlay

Source colors overlay the destination.

case darken

Use the darker of the source and destination colors.

case lighten

Use the lighter of the source and destination colors.

case colorDodge

Brightens the destination to reflect the source.

case colorBurn

Darkens the destination color to reflect the source.

case softLight

Darkens or lightens colors, with the effect of shining a diffused spotlight on the destination.

case hardLight

Multiplies or screens colors, with the effect of shining a spotlight on the destination.

case difference

Subtracts the darker value from the lighter value.

case exclusion

Subtracts the darker value from the lighter value, except lower in contrast.

case hue

Uses the hue of the source and the saturation and luminosity of the destination.

case saturation

Uses the saturation value of the source and the hue and luminosity of the destination.

case color

Uses the hue and saturation of the source and the luminosity of the destination.

case luminosity

Uses the luminosity of the source and the hue and saturation of the destination.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring Rendering Options

var compositingOperation: NSCompositingOperation

The graphics context’s global compositing operation setting.

var imageInterpolation: NSImageInterpolation

A constant that specifies the graphics context’s interpolation, or image smoothing, behavior.

enum NSImageInterpolation

Constants that specify the interpolation, or image smoothing, behavior used by the image interpolation property.

var shouldAntialias: Bool

A Boolean value that indicates whether the graphics context uses antialiasing.

var patternPhase: NSPoint

The amount to offset the pattern color when filling the graphics context.

