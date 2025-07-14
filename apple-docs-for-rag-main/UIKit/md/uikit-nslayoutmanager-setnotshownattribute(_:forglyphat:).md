

- UIKit
- NSLayoutManager
-  setNotShownAttribute(\_:forGlyphAt:) 

Instance Method

# setNotShownAttribute(\_:forGlyphAt:)

Sets the visibility of the glyph at the specified index.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
func setNotShownAttribute(
    _ flag: Bool,
    forGlyphAt glyphIndex: Int
)
```

## Parameters 

`flag`  

If true, the glyph is not shown; if false, it is shown.

`glyphIndex`  

Index of the glyph whose attribute is set.

## Discussion

The typesetter decides which glyphs are not shown and sets this attribute in the layout manager to ensure that those glyphs are not displayed. For example, a tab or newline character doesn’t leave any marks; it just indicates where following glyphs are laid out.

Raises an `NSRangeException` if `glyphIndex` is out of bounds.

This method is used by the layout mechanism and should be invoked only during typesetting, in almost all cases only by the typesetter. For example, a custom typesetter might invoke it.

## See Also

### Related Documentation

func notShownAttribute(forGlyphAt: Int) -> Bool

Indicates whether the glyph at the specified index has a visible representation.

### Setting layout information

func setAttachmentSize(CGSize, forGlyphRange: NSRange)

Sets the size to use when drawing a glyph that represents an attachment.

func setDrawsOutsideLineFragment(Bool, forGlyphAt: Int)

Indicates whether the specified glyph exceeds the bounds of the line fragment for its layout.

func setExtraLineFragmentRect(CGRect, usedRect: CGRect, textContainer: NSTextContainer)

Sets the bounds and container for the extra line fragment.

func setLineFragmentRect(CGRect, forGlyphRange: NSRange, usedRect: CGRect)

Associates the line fragment bounds for the specified range of glyphs.

func setLocation(CGPoint, forStartOfGlyphRange: NSRange)

Sets the location for the first glyph in the specified range.

