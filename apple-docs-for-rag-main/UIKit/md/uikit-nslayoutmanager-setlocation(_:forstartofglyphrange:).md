

- UIKit
- NSLayoutManager
-  setLocation(\_:forStartOfGlyphRange:) 

Instance Method

# setLocation(\_:forStartOfGlyphRange:)

Sets the location for the first glyph in the specified range.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
func setLocation(
    _ location: CGPoint,
    forStartOfGlyphRange glyphRange: NSRange
)
```

## Parameters 

`location`  

The location to which the first glyph is set, relative to the origin of the glyph’s line fragment origin.

`glyphRange`  

The glyphs whose location is set.

## Discussion

Setting the location for a glyph range implies that its first glyph is not nominally spaced with respect to the previous glyph. In the course of layout, all glyphs should end up being included in a range passed to this method, but only glyphs that start a new nominal range should be at the start of such ranges. The first glyph in a line fragment should always start a new nominal range. Glyph locations are given relative to their line fragment rectangle’s origin.

Before setting the location for a glyph range, you must specify the text container with setTextContainer(_:forGlyphRange:) and the line fragment rectangle with setLineFragmentRect(_:forGlyphRange:usedRect:).

This method is used by the layout mechanism and should be invoked only during typesetting, in almost all cases only by the typesetter. For example, a custom typesetter might invoke it.

## See Also

### Setting layout information

func setAttachmentSize(CGSize, forGlyphRange: NSRange)

Sets the size to use when drawing a glyph that represents an attachment.

func setDrawsOutsideLineFragment(Bool, forGlyphAt: Int)

Indicates whether the specified glyph exceeds the bounds of the line fragment for its layout.

func setExtraLineFragmentRect(CGRect, usedRect: CGRect, textContainer: NSTextContainer)

Sets the bounds and container for the extra line fragment.

func setLineFragmentRect(CGRect, forGlyphRange: NSRange, usedRect: CGRect)

Associates the line fragment bounds for the specified range of glyphs.

func setNotShownAttribute(Bool, forGlyphAt: Int)

Sets the visibility of the glyph at the specified index.

