

- Core Animation
- CATextLayer
-  allowsFontSubpixelQuantization 

Instance Property

# allowsFontSubpixelQuantization

Determines whether to allow subpixel quantization for the graphics context used for text rendering.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var allowsFontSubpixelQuantization: Bool { get set }
```

## Discussion

When enabled, the graphics context used for text rendering may quantize the subpixel positions of glyphs.

## See Also

### Text Visual Properties

var font: CFTypeRef?

The font used to render the receiver’s text.

var fontSize: CGFloat

The font size used to render the receiver’s text. Animatable.

var foregroundColor: CGColor?

The color used to render the receiver’s text. Animatable.

