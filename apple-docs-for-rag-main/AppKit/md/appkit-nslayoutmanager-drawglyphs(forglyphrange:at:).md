

- AppKit
- NSLayoutManager
-  drawGlyphs(forGlyphRange:at:) 

Instance Method

# drawGlyphs(forGlyphRange:at:)

Draws the specified glyphs, which must lie completely within a single text container.

macOS 10.7+

``` source
func drawGlyphs(
    forGlyphRange glyphsToShow: NSRange,
    at origin: NSPoint
)
```

## Parameters 

`glyphsToShow`  

The range of glyphs that are drawn.

`origin`  

The position of the text container in the coordinate system of the currently focused view.

## Discussion

This method is called by `NSTextView` for drawing. You can override it to perform additional drawing, or to replace text drawing entirely, but not to change layout. You can call this method directly, but focus must already be locked on the destination view or image. This method expects the coordinate system of the view to be flipped.

This method draws the actual glyphs, including attachments, as well as any underlines or strikethoughs.

Performs glyph generation and layout if needed.

## See Also

### Drawing

func drawBackground(forGlyphRange: NSRange, at: NSPoint)

Draws background marks for the specified glyphs, which must lie completely within a single text container.

func drawStrikethrough(forGlyphRange: NSRange, strikethroughType: NSUnderlineStyle, baselineOffset: CGFloat, lineFragmentRect: NSRect, lineFragmentGlyphRange: NSRange, containerOrigin: NSPoint)

Draws a strikethrough for the specified glyphs.

func drawUnderline(forGlyphRange: NSRange, underlineType: NSUnderlineStyle, baselineOffset: CGFloat, lineFragmentRect: NSRect, lineFragmentGlyphRange: NSRange, containerOrigin: NSPoint)

Draws underlining for the glyphs in a specified range.

func fillBackgroundRectArray(UnsafePointer&lt;NSRect>, count: Int, forCharacterRange: NSRange, color: NSColor)

Fills background rectangles with a color.

func showCGGlyphs(UnsafePointer&lt;CGGlyph>, positions: UnsafePointer&lt;CGPoint>, count: Int, font: NSFont, textMatrix: CGAffineTransform, attributes: [NSAttributedString.Key : Any], in: CGContext)

Renders the glyphs at the specified positions, using the specified attributes.

func strikethroughGlyphRange(NSRange, strikethroughType: NSUnderlineStyle, lineFragmentRect: NSRect, lineFragmentGlyphRange: NSRange, containerOrigin: NSPoint)

Calculates and draws strikethrough for the specified glyphs.

func underlineGlyphRange(NSRange, underlineType: NSUnderlineStyle, lineFragmentRect: NSRect, lineFragmentGlyphRange: NSRange, containerOrigin: NSPoint)

Calculates subranges to underline for the specified glyphs and draws the underlining as appropriate.

