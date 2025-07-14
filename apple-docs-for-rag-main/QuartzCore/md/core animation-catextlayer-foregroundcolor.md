

- Core Animation
- CATextLayer
-  foregroundColor 

Instance Property

# foregroundColor

The color used to render the receiver’s text. Animatable.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var foregroundColor: CGColor? { get set }
```

## Discussion

Defaults to opaque white.

The `foregroundColor` property is only used when the string property is not an `NSAttributedString`.

Note

Implicit animation of this property is only enabled in applications compiled for macOS 10.6 and later.

## See Also

### Text Visual Properties

var font: CFTypeRef?

The font used to render the receiver’s text.

var fontSize: CGFloat

The font size used to render the receiver’s text. Animatable.

var allowsFontSubpixelQuantization: Bool

Determines whether to allow subpixel quantization for the graphics context used for text rendering.

