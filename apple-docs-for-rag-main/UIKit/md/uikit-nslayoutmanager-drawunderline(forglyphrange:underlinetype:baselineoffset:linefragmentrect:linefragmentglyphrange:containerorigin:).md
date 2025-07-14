

- UIKit
- NSLayoutManager
-  drawUnderline(forGlyphRange:underlineType:baselineOffset:lineFragmentRect:lineFragmentGlyphRange:containerOrigin:) 

Instance Method

# drawUnderline(forGlyphRange:underlineType:baselineOffset:lineFragmentRect:lineFragmentGlyphRange:containerOrigin:)

Draws underlining for the glyphs in a specified range.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
func drawUnderline(
    forGlyphRange glyphRange: NSRange,
    underlineType underlineVal: NSUnderlineStyle,
    baselineOffset: CGFloat,
    lineFragmentRect lineRect: CGRect,
    lineFragmentGlyphRange lineGlyphRange: NSRange,
    containerOrigin: CGPoint
)
```

## Parameters 

`glyphRange`  

A range of glyphs, which must belong to a single line fragment rectangle (as returned by lineFragmentRect(forGlyphAt:effectiveRange:)).

`underlineVal`  

The style of underlining to draw. This value is a mask derived from the value for NSUnderlineStyleAttributeName—for example, `(NSUnderlinePatternDash | NSUnderlineStyleThick)`. Subclasses can define custom underlining styles.

`baselineOffset`  

Specifies the distance from the bottom of the bounding box of the specified glyphs in the specified range to their baseline.

`lineRect`  

The line fragment rectangle containing the glyphs to draw underlining for.

`lineGlyphRange`  

The range of all glyphs within `lineRect`.

`containerOrigin`  

The origin of the `lineRectNSTextContainer` in its `NSTextView`.

## Discussion

This method is invoked automatically by underlineGlyphRange(_:underlineType:lineFragmentRect:lineFragmentGlyphRange:containerOrigin:); you should rarely need to invoke it directly. This method’s `underlineVal` parameter does not take account of any setting for NSUnderlineByWordMask because that’s taken care of by underlineGlyphRange(_:underlineType:lineFragmentRect:lineFragmentGlyphRange:containerOrigin:).

## See Also

### Drawing

func drawBackground(forGlyphRange: NSRange, at: CGPoint)

Draws background marks for the specified glyphs, which must lie completely within a single text container.

func drawGlyphs(forGlyphRange: NSRange, at: CGPoint)

Draws the specified glyphs, which must lie completely within a single text container.

func drawStrikethrough(forGlyphRange: NSRange, strikethroughType: NSUnderlineStyle, baselineOffset: CGFloat, lineFragmentRect: CGRect, lineFragmentGlyphRange: NSRange, containerOrigin: CGPoint)

Draws a strikethrough for the specified glyphs.

func fillBackgroundRectArray(UnsafePointer&lt;CGRect>, count: Int, forCharacterRange: NSRange, color: UIColor)

Fills background rectangles with a color.

func showCGGlyphs(UnsafePointer&lt;CGGlyph>, positions: UnsafePointer&lt;CGPoint>, count: Int, font: UIFont, textMatrix: CGAffineTransform, attributes: [NSAttributedString.Key : Any], in: CGContext)

Renders the glyphs at the specified positions, using the specified attributes.

func strikethroughGlyphRange(NSRange, strikethroughType: NSUnderlineStyle, lineFragmentRect: CGRect, lineFragmentGlyphRange: NSRange, containerOrigin: CGPoint)

Calculates and draws strikethrough for the specified glyphs.

func underlineGlyphRange(NSRange, underlineType: NSUnderlineStyle, lineFragmentRect: CGRect, lineFragmentGlyphRange: NSRange, containerOrigin: CGPoint)

Calculates subranges to underline for the specified glyphs and draws the underlining as appropriate.

