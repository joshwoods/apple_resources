

- Core Graphics
- CGContext
-  setAllowsFontSmoothing(\_:) 

Instance Method

# setAllowsFontSmoothing(\_:)

Sets whether or not to allow font smoothing for a graphics context.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func setAllowsFontSmoothing(_ allowsFontSmoothing: Bool)
```

## Parameters 

`allowsFontSmoothing`  

A Boolean value that specifies whether font smoothing is allowed in the specified context.

## Discussion

Font are smoothed if they are antialiased when drawn and if font smoothing is both allowed and enabled. For information on how to enable font smoothing, see the setShouldSmoothFonts(_:) function. It is not usually necessary to make changes to both parameters at the same time; either can be used to disable font smoothing.

This parameter is not part of the graphics state.

## See Also

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

func showGlyphsAtPoint(x: CGFloat, y: CGFloat, glyphs: UnsafePointer&lt;CGGlyph>?, count: Int)

Displays an array of glyphs at a position you specify.

Deprecated

