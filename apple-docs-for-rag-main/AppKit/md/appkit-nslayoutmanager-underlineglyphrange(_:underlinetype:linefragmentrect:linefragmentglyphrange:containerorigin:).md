

- AppKit
- NSLayoutManager
-  underlineGlyphRange(\_:underlineType:lineFragmentRect:lineFragmentGlyphRange:containerOrigin:) 

Instance Method

# underlineGlyphRange(\_:underlineType:lineFragmentRect:lineFragmentGlyphRange:containerOrigin:)

Calculates subranges to underline for the specified glyphs and draws the underlining as appropriate.

macOS 10.7+

``` source
func underlineGlyphRange(
    _ glyphRange: NSRange,
    underlineType underlineVal: NSUnderlineStyle,
    lineFragmentRect lineRect: NSRect,
    lineFragmentGlyphRange lineGlyphRange: NSRange,
    containerOrigin: NSPoint
)
```

## Parameters 

`glyphRange`  

A range of glyphs, which must belong to a single line fragment rectangle (as returned by lineFragmentRect(forGlyphAt:effectiveRange:)).

`underlineVal`  

The style of underlining to draw. This value is a mask derived from the value for underlineStyle—for example, `(NSUnderlinePatternDash | NSUnderlineStyleThick | NSUnderlineByWordMask)`. Subclasses can define custom underlining styles.

`lineRect`  

The line fragment rectangle containing the glyphs to draw underlining for.

`lineGlyphRange`  

The range of all glyphs within that line fragment rectangle.

`containerOrigin`  

The origin of the line fragment rectangle’s `NSTextContainer` in its `NSTextView`.

## Discussion

This method determines which glyphs actually need to be underlined based on `underlineVal`. With `NSUnderlineStyleSingle`, for example, leading and trailing whitespace isn’t underlined, but whitespace between visible glyphs is. A potential word-underline style would omit underlining on any whitespace. After determining which glyphs to draw underlining on, this method invokes drawUnderline(forGlyphRange:underlineType:baselineOffset:lineFragmentRect:lineFragmentGlyphRange:containerOrigin:) for each contiguous range of glyphs that requires it.

## See Also

### Drawing

func drawBackground(forGlyphRange: NSRange, at: NSPoint)

Draws background marks for the specified glyphs, which must lie completely within a single text container.

func drawGlyphs(forGlyphRange: NSRange, at: NSPoint)

Draws the specified glyphs, which must lie completely within a single text container.

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

