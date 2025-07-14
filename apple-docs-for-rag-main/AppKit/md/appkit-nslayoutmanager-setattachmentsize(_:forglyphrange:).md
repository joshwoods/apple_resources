

- AppKit
- NSLayoutManager
-  setAttachmentSize(\_:forGlyphRange:) 

Instance Method

# setAttachmentSize(\_:forGlyphRange:)

Sets the size to use when drawing a glyph that represents an attachment.

macOS 10.7+

``` source
func setAttachmentSize(
    _ attachmentSize: NSSize,
    forGlyphRange glyphRange: NSRange
)
```

## Parameters 

`attachmentSize`  

The glyph size to set.

`glyphRange`  

The attachment glyph’s position in the glyph stream.

## Discussion

For a glyph corresponding to an attachment, this method should be called to set the size for the attachment cell to occupy. The glyph’s value should be NSControlGlyph.

This method is used by the layout mechanism and should be invoked only during typesetting, in almost all cases only by the typesetter. For example, a custom typesetter might invoke it.

## See Also

### Setting layout information

func setDrawsOutsideLineFragment(Bool, forGlyphAt: Int)

Indicates whether the specified glyph exceeds the bounds of the line fragment for its layout.

func setExtraLineFragmentRect(NSRect, usedRect: NSRect, textContainer: NSTextContainer)

Sets the bounds and container for the extra line fragment.

func setLineFragmentRect(NSRect, forGlyphRange: NSRange, usedRect: NSRect)

Associates the line fragment bounds for the specified range of glyphs.

func setLocation(NSPoint, forStartOfGlyphRange: NSRange)

Sets the location for the first glyph in the specified range.

func setNotShownAttribute(Bool, forGlyphAt: Int)

Sets the visibility of the glyph at the specified index.

