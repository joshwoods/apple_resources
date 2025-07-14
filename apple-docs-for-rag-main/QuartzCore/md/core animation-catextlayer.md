

- Core Animation
-  CATextLayer 

Class

# CATextLayer

A layer that provides simple text layout and rendering of plain or attributed strings.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
class CATextLayer
```

## Overview

The first line is aligned to the top of the layer.

Note

`CATextLayer` disables sub-pixel antialiasing when rendering text. Text can only be drawn using sub-pixel antialiasing when it is composited into an existing opaque background at the same time that it’s rasterized. There is no way to draw text with sub-pixel antialiasing by itself, whether into an image or a layer, in advance of having the background pixels to weave the text pixels into. Setting the `opacity` property of the layer to true does not change the rendering mode.

Note

In macOS, when a `CATextLayer` instance is positioned using the CAConstraintLayoutManager class the bounds of the layer is resized to fit the text content.

## Topics

### Getting and Setting the Text

var string: Any?

The text to be rendered by the receiver.

### Text Visual Properties

var font: CFTypeRef?

The font used to render the receiver’s text.

var fontSize: CGFloat

The font size used to render the receiver’s text. Animatable.

var foregroundColor: CGColor?

The color used to render the receiver’s text. Animatable.

var allowsFontSubpixelQuantization: Bool

Determines whether to allow subpixel quantization for the graphics context used for text rendering.

### Text Alignment and Truncation

var isWrapped: Bool

Determines whether the text is wrapped to fit within the receiver’s bounds.

var alignmentMode: CATextLayerAlignmentMode

Determines how individual lines of text are horizontally aligned within the receiver’s bounds.

var truncationMode: CATextLayerTruncationMode

Determines how the text is truncated to fit within the receiver’s bounds.

### Constants

Truncation modes

These constants are used by the truncationMode property.

Horizontal alignment modes

These constants are used by the alignmentMode property.

## Relationships

### Inherits From

- CALayer

### Conforms To

- CAMediaTiming
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Text, Shapes, and Gradients

class CAShapeLayer

A layer that draws a cubic Bezier spline in its coordinate space.

class CAGradientLayer

A layer that draws a color gradient over its background color, filling the shape of the layer.

