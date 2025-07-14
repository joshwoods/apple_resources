

- UIKit
- NSLayoutManager
-  fillBackgroundRectArray(\_:count:forCharacterRange:color:) 

Instance Method

# fillBackgroundRectArray(\_:count:forCharacterRange:color:)

Fills background rectangles with a color.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
func fillBackgroundRectArray(
    _ rectArray: UnsafePointer,
    count rectCount: Int,
    forCharacterRange charRange: NSRange,
    color: UIColor
)
```

## Parameters 

`rectArray`  

The array of rectangles to fill.

`rectCount`  

The number of rectangles in `rectArray`.

`charRange`  

The range of characters whose background rectangles are filled.

`color`  

The fill color.

## Discussion

This is the primitive method used by drawBackground(forGlyphRange:at:), providing a finer-grained override point for actually filling rectangles with a particular background color for a background color attribute, a selected or marked range highlight, a block decoration, or any other rectangle fill needed by that method. As with showPackedGlyphs:length:glyphRange:atPoint:font:color:printingAdjustment:, the `charRange` and `color` parameters are passed in merely for informational purposes; the color is already set in the graphics state. If for any reason you modify it, you must restore it before returning from this method.

This method operates in terms of character ranges, because the relevant attributes are expressed on characters, and they don’t always lie on glyph boundaries—for example, when one character of an “fi” ligature is highlighted.

You should never call this method, but you might override it. The default implementation simply fills the rectangles in the specified array. The graphics operation used for this fill is controlled by a link check; for compatibility reasons, it is NSCompositeCopy for applications linked prior to OS X v10.6 and NSCompositeSourceOver for applications linked on macOS 10.6 or later. Applications can control the operation used, or modify the drawing, by overriding this method in an `NSLayoutManager` subclass.

## See Also

### Drawing

func drawBackground(forGlyphRange: NSRange, at: CGPoint)

Draws background marks for the specified glyphs, which must lie completely within a single text container.

func drawGlyphs(forGlyphRange: NSRange, at: CGPoint)

Draws the specified glyphs, which must lie completely within a single text container.

func drawStrikethrough(forGlyphRange: NSRange, strikethroughType: NSUnderlineStyle, baselineOffset: CGFloat, lineFragmentRect: CGRect, lineFragmentGlyphRange: NSRange, containerOrigin: CGPoint)

Draws a strikethrough for the specified glyphs.

func drawUnderline(forGlyphRange: NSRange, underlineType: NSUnderlineStyle, baselineOffset: CGFloat, lineFragmentRect: CGRect, lineFragmentGlyphRange: NSRange, containerOrigin: CGPoint)

Draws underlining for the glyphs in a specified range.

func showCGGlyphs(UnsafePointer&lt;CGGlyph>, positions: UnsafePointer&lt;CGPoint>, count: Int, font: UIFont, textMatrix: CGAffineTransform, attributes: [NSAttributedString.Key : Any], in: CGContext)

Renders the glyphs at the specified positions, using the specified attributes.

func strikethroughGlyphRange(NSRange, strikethroughType: NSUnderlineStyle, lineFragmentRect: CGRect, lineFragmentGlyphRange: NSRange, containerOrigin: CGPoint)

Calculates and draws strikethrough for the specified glyphs.

func underlineGlyphRange(NSRange, underlineType: NSUnderlineStyle, lineFragmentRect: CGRect, lineFragmentGlyphRange: NSRange, containerOrigin: CGPoint)

Calculates subranges to underline for the specified glyphs and draws the underlining as appropriate.

