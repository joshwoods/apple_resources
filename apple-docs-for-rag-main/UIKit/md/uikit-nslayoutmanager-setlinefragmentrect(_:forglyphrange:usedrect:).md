

- UIKit
- NSLayoutManager
-  setLineFragmentRect(\_:forGlyphRange:usedRect:) 

Instance Method

# setLineFragmentRect(\_:forGlyphRange:usedRect:)

Associates the line fragment bounds for the specified range of glyphs.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
func setLineFragmentRect(
    _ fragmentRect: CGRect,
    forGlyphRange glyphRange: NSRange,
    usedRect: CGRect
)
```

## Parameters 

`fragmentRect`  

The rectangle of the line fragment.

`glyphRange`  

The range of glyphs to be associated with `fragmentRect`.

`usedRect`  

The portion of `fragmentRect` that actually contains glyphs or other marks that are drawn (including the text container’s line fragment padding. Must be equal to or contained within `fragmentRect`.

## Discussion

The typesetter must specify the text container first with setTextContainer(_:forGlyphRange:), and it sets the exact positions of the glyphs afterwards with setLocation(_:forStartOfGlyphRange:).

In the course of layout, all glyphs should end up being included in a range passed to this method, but only glyphs that start a new line fragment should be at the start of such ranges.

Line fragment rectangles and line fragment used rectangles are always in container coordinates.

This method is used by the layout mechanism and should be invoked only during typesetting, in almost all cases only by the typesetter. For example, a custom typesetter might invoke it.

## See Also

### Related Documentation

func lineFragmentUsedRect(forGlyphAt: Int, effectiveRange: NSRangePointer?, withoutAdditionalLayout: Bool) -> CGRect

Returns the usage rectangle for the line fragment and (optionally) returns the entire range of glyphs in that fragment.

func lineFragmentRect(forGlyphAt: Int, effectiveRange: NSRangePointer?) -> CGRect

Returns the rectangle for the line fragment where the glyph lies and (optionally), by reference, the entire range of glyphs in that fragment.

func lineFragmentRect(forGlyphAt: Int, effectiveRange: NSRangePointer?, withoutAdditionalLayout: Bool) -> CGRect

Returns the line fragment rectangle that contains the glyph at the specified glyph index.

func lineFragmentUsedRect(forGlyphAt: Int, effectiveRange: NSRangePointer?) -> CGRect

Returns the usage rectangle for the line fragment and (optionally) returns the entire range of glyphs in that fragment.

### Setting layout information

func setAttachmentSize(CGSize, forGlyphRange: NSRange)

Sets the size to use when drawing a glyph that represents an attachment.

func setDrawsOutsideLineFragment(Bool, forGlyphAt: Int)

Indicates whether the specified glyph exceeds the bounds of the line fragment for its layout.

func setExtraLineFragmentRect(CGRect, usedRect: CGRect, textContainer: NSTextContainer)

Sets the bounds and container for the extra line fragment.

func setLocation(CGPoint, forStartOfGlyphRange: NSRange)

Sets the location for the first glyph in the specified range.

func setNotShownAttribute(Bool, forGlyphAt: Int)

Sets the visibility of the glyph at the specified index.

