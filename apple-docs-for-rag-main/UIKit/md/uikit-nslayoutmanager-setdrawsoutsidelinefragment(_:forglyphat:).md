

- UIKit
- NSLayoutManager
-  setDrawsOutsideLineFragment(\_:forGlyphAt:) 

Instance Method

# setDrawsOutsideLineFragment(\_:forGlyphAt:)

Indicates whether the specified glyph exceeds the bounds of the line fragment for its layout.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
func setDrawsOutsideLineFragment(
    _ flag: Bool,
    forGlyphAt glyphIndex: Int
)
```

## Parameters 

`flag`  

If true, sets the given glyph to draw outside its line fragment; if false, the glyph does not draw outside.

`glyphIndex`  

Index of the glyph to set.

## Discussion

This can happen when text is set at a fixed line height. For example, if the user specifies a fixed line height of 12 points and sets the font size to 24 points, the glyphs will exceed their layout rectangles. This information is important for determining whether additional lines need to be redrawn as a result of changes to any given line fragment.

This method is used by the layout mechanism and should be invoked only during typesetting, in almost all cases only by the typesetter. For example, a custom typesetter might invoke it.

## See Also

### Related Documentation

func drawsOutsideLineFragment(forGlyphAt: Int) -> Bool

Indicates whether the glyph draws outside its line fragment rectangle.

### Setting layout information

func setAttachmentSize(CGSize, forGlyphRange: NSRange)

Sets the size to use when drawing a glyph that represents an attachment.

func setExtraLineFragmentRect(CGRect, usedRect: CGRect, textContainer: NSTextContainer)

Sets the bounds and container for the extra line fragment.

func setLineFragmentRect(CGRect, forGlyphRange: NSRange, usedRect: CGRect)

Associates the line fragment bounds for the specified range of glyphs.

func setLocation(CGPoint, forStartOfGlyphRange: NSRange)

Sets the location for the first glyph in the specified range.

func setNotShownAttribute(Bool, forGlyphAt: Int)

Sets the visibility of the glyph at the specified index.

