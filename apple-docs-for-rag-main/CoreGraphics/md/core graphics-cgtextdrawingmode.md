

- Core Graphics
-  CGTextDrawingMode 

Enumeration

# CGTextDrawingMode

Modes for rendering text.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum CGTextDrawingMode
```

## Overview

You provide a text drawing mode constant to the function setTextDrawingMode(_:) to set the current text drawing mode for a graphics context. Text drawing modes determine how Core Graphics renders individual glyphs onscreen. For example, you can set a text drawing mode to draw text filled in or outlined (stroked) or both. You can also create special effects with the text clipping drawing modes, such as clipping an image to a glyph shape.

## Topics

### Constants

case fill

Perform a fill operation on the text.

case stroke

Perform a stroke operation on the text.

case fillStroke

Perform fill, then stroke operations on the text.

case invisible

Do not draw the text, but do update the text position.

case fillClip

Perform a fill operation, then intersect the text with the current clipping path.

case strokeClip

Perform a stroke operation, then intersect the text with the current clipping path.

case fillStrokeClip

Perform fill then stroke operations, then intersect the text with the current clipping path.

case clip

Specifies to intersect the text with the current clipping path. This mode does not paint the text.

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

