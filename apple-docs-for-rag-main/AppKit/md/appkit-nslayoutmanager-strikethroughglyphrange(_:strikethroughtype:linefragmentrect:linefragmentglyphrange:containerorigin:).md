

- AppKit
- NSLayoutManager
-  strikethroughGlyphRange(\_:strikethroughType:lineFragmentRect:lineFragmentGlyphRange:containerOrigin:) 

Instance Method

# strikethroughGlyphRange(\_:strikethroughType:lineFragmentRect:lineFragmentGlyphRange:containerOrigin:)

Calculates and draws strikethrough for the specified glyphs.

macOS 10.7+

``` source
func strikethroughGlyphRange(
    _ glyphRange: NSRange,
    strikethroughType strikethroughVal: NSUnderlineStyle,
    lineFragmentRect lineRect: NSRect,
    lineFragmentGlyphRange lineGlyphRange: NSRange,
    containerOrigin: NSPoint
)
```

## Parameters 

`glyphRange`  

The range of glyphs for which to draw a strikethrough. The range must belong to a single line fragment rectangle (as returned by lineFragmentRect(forGlyphAt:effectiveRange:)).

`strikethroughVal`  

The style of underlining to draw. This value is a mask derived from the value for underlineStyle—for example, `(NSUnderlinePatternDash | NSUnderlineStyleThick | NSUnderlineByWordMask)`. Subclasses can define custom underlining styles.

`lineRect`  

The line fragment rectangle containing the glyphs to draw strikethrough for.

`lineGlyphRange`  

The range of all glyphs within `lineRect`.

`containerOrigin`  

The origin of the line fragment rectangle’s `NSTextContainer` in its `NSTextView`.

## Discussion

This method determines which glyphs actually need to have a strikethrough drawn based on `strikethroughVal`. After determining which glyphs to draw strikethrough on, this method invokes drawStrikethrough(forGlyphRange:strikethroughType:baselineOffset:lineFragmentRect:lineFragmentGlyphRange:containerOrigin:) for each contiguous range of glyphs that requires it.

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

func underlineGlyphRange(NSRange, underlineType: NSUnderlineStyle, lineFragmentRect: NSRect, lineFragmentGlyphRange: NSRange, containerOrigin: NSPoint)

Calculates subranges to underline for the specified glyphs and draws the underlining as appropriate.

