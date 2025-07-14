

- AppKit
- NSLayoutManager
-  drawStrikethrough(forGlyphRange:strikethroughType:baselineOffset:lineFragmentRect:lineFragmentGlyphRange:containerOrigin:) 

Instance Method

# drawStrikethrough(forGlyphRange:strikethroughType:baselineOffset:lineFragmentRect:lineFragmentGlyphRange:containerOrigin:)

Draws a strikethrough for the specified glyphs.

macOS 10.7+

``` source
func drawStrikethrough(
    forGlyphRange glyphRange: NSRange,
    strikethroughType strikethroughVal: NSUnderlineStyle,
    baselineOffset: CGFloat,
    lineFragmentRect lineRect: NSRect,
    lineFragmentGlyphRange lineGlyphRange: NSRange,
    containerOrigin: NSPoint
)
```

## Parameters 

`glyphRange`  

The range of glyphs for which to draw a strikethrough. The range must belong to a single line fragment rectangle (as returned by lineFragmentRect(forGlyphAt:effectiveRange:)).

`strikethroughVal`  

The style of strikethrough to draw. This value is a mask derived from the value for underlineStyle—for example, `(NSUnderlinePatternDash | NSUnderlineStyleThick)`. Subclasses can define custom strikethrough styles.

`baselineOffset`  

Indicates how far above the text baseline the underline should be drawn.

`lineRect`  

The line fragment rectangle containing the glyphs to draw strikethrough for.

`lineGlyphRange`  

The range of all glyphs within `lineRect`.

`containerOrigin`  

The origin of the line fragment rectangle’s `NSTextContainer` in its `NSTextView`.

## Discussion

This method is invoked automatically by strikethroughGlyphRange(_:strikethroughType:lineFragmentRect:lineFragmentGlyphRange:containerOrigin:); you should rarely need to invoke it directly. This method’s `strikethroughVal` parameter does not take account of any setting forNSUnderlineByWordMask because that’s taken care of by underlineGlyphRange(_:underlineType:lineFragmentRect:lineFragmentGlyphRange:containerOrigin:).

## See Also

### Drawing

func drawBackground(forGlyphRange: NSRange, at: NSPoint)

Draws background marks for the specified glyphs, which must lie completely within a single text container.

func drawGlyphs(forGlyphRange: NSRange, at: NSPoint)

Draws the specified glyphs, which must lie completely within a single text container.

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

