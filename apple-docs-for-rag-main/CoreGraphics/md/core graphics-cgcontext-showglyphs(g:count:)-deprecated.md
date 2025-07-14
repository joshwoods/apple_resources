

- Core Graphics
- CGContext
-  showGlyphs(g:count:) Deprecated

Instance Method

# showGlyphs(g:count:)

Displays an array of glyphs at the current text position.

tvOSvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
func showGlyphs(
    g: UnsafePointer?,
    count: Int
)
```

Deprecated

Use Core Text instead.

## Parameters 

`g`  

An array of glyphs to display.

`count`  

The total number of glyphs passed in the `g` parameter.

## Discussion

This function displays an array of glyphs at the current text position, a point specified by the current text matrix.

## See Also

### Related Documentation

func showText(string: UnsafePointer&lt;CChar>, length: Int)

Displays a character array at the current text position, a point specified by the current text matrix.

Deprecated

func showTextAtPoint(x: CGFloat, y: CGFloat, string: UnsafePointer&lt;CChar>, length: Int)

Displays a character string at a position you specify.

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

func showGlyphs([CGGlyph], at: [CGPoint])

Draws a set of glyphs at a set of corresponding positions.

func showGlyphsAtPoint(x: CGFloat, y: CGFloat, glyphs: UnsafePointer&lt;CGGlyph>?, count: Int)

Displays an array of glyphs at a position you specify.

Deprecated

