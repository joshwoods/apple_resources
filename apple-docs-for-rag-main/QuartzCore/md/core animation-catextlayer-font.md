

- Core Animation
- CATextLayer
-  font 

Instance Property

# font

The font used to render the receiver’s text.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var font: CFTypeRef? { get set }
```

## Discussion

May be either a CTFont, a CGFont, an instance of `NSFont` (macOS only), or a string naming the font. In iOS, you cannot assign a UIFont object to this property. Defaults to Helvetica.

The `font` property is only used when the string property is not an `NSAttributedString`.

Note

If the font property is a `CTFontRef`, a `CGFontRef`, or an instance of `NSFont`, the font size of the property is ignored.

## See Also

### Text Visual Properties

var fontSize: CGFloat

The font size used to render the receiver’s text. Animatable.

var foregroundColor: CGColor?

The color used to render the receiver’s text. Animatable.

var allowsFontSubpixelQuantization: Bool

Determines whether to allow subpixel quantization for the graphics context used for text rendering.

