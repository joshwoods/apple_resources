

- Core Graphics
- CGContext
-  showTextAtPoint(x:y:string:length:) Deprecated

Instance Method

# showTextAtPoint(x:y:string:length:)

Displays a character string at a position you specify.

tvOSvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
func showTextAtPoint(
    x: CGFloat,
    y: CGFloat,
    string: UnsafePointer,
    length: Int
)
```

Deprecated

Use Core Text instead.

## Parameters 

`x`  

A value for the x-coordinate (in user space) at which to display the text.

`y`  

A value for the y-coordinate (in user space) at which to display the text.

`string`  

An array of characters to draw.

`length`  

The length of the array specified in the `string` parameter.

## Discussion

Core Graphics uses font data provided by the system to map each byte of the array through the encoding vector of the current font to obtain the glyph to display. Note that the font must have been set using selectFont(name:size:textEncoding:). Don’t use `CGContextShowTextAtPoint` in conjunction with setFont(_:).

## See Also

### Related Documentation

func showGlyphsAtPoint(x: CGFloat, y: CGFloat, glyphs: UnsafePointer&lt;CGGlyph>?, count: Int)

Displays an array of glyphs at a position you specify.

Deprecated

func showGlyphs(g: UnsafePointer&lt;CGGlyph>?, count: Int)

Displays an array of glyphs at the current text position.

Deprecated

func showGlyphsWithAdvances(glyphs: UnsafePointer&lt;CGGlyph>?, advances: UnsafePointer&lt;CGSize>?, count: Int)

Draws an array of glyphs with varying offsets.

Deprecated

### Drawing Text

var textMatrix: CGAffineTransform

Returns the current text matrix.

var textPosition: CGPoint

Returns the location at which text is drawn.

func selectFont(name: UnsafePointer&lt;CChar>, size: CGFloat, textEncoding: CGTextEncoding)

Sets the font and font size in a graphics context.

Deprecated

func setCharacterSpacing(CGFloat)

Sets the current character spacing.

func setFont(CGFont)

Sets the platform font in a graphics context.

func setFontSize(CGFloat)

Sets the current font size.

func setTextDrawingMode(CGTextDrawingMode)

Sets the current text drawing mode.

func setAllowsFontSmoothing(Bool)

Sets whether or not to allow font smoothing for a graphics context.

func setAllowsFontSubpixelPositioning(Bool)

Sets whether or not to allow subpixel positioning for a graphics context.

func setAllowsFontSubpixelQuantization(Bool)

Sets whether or not to allow subpixel quantization for a graphics context.

func setShouldSmoothFonts(Bool)

Enables or disables font smoothing in a graphics context.

func setShouldSubpixelPositionFonts(Bool)

Enables or disables subpixel positioning in a graphics context.

func setShouldSubpixelQuantizeFonts(Bool)

Enables or disables subpixel quantization in a graphics context.

func showGlyphs(g: UnsafePointer&lt;CGGlyph>?, count: Int)

Displays an array of glyphs at the current text position.

Deprecated

func showGlyphs([CGGlyph], at: [CGPoint])

Draws a set of glyphs at a set of corresponding positions.

