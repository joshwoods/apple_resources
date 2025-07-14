

- UIKit
- NSLayoutManager
-  setAttachmentSize(\_:forGlyphRange:) 

Instance Method

# setAttachmentSize(\_:forGlyphRange:)

Sets the size to use when drawing a glyph that represents an attachment.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
func setAttachmentSize(
    _ attachmentSize: CGSize,
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

### Related Documentation

func attachmentSize(forGlyphAt: Int) -> CGSize

Returns the size of the attachment glyph at the specified index.

var defaultAttachmentScaling: NSImageScaling { get set }

The default amount of scaling to apply when an attachment image is too large to fit in a text container.

### Setting layout information

func setDrawsOutsideLineFragment(Bool, forGlyphAt: Int)

Indicates whether the specified glyph exceeds the bounds of the line fragment for its layout.

func setExtraLineFragmentRect(CGRect, usedRect: CGRect, textContainer: NSTextContainer)

Sets the bounds and container for the extra line fragment.

func setLineFragmentRect(CGRect, forGlyphRange: NSRange, usedRect: CGRect)

Associates the line fragment bounds for the specified range of glyphs.

func setLocation(CGPoint, forStartOfGlyphRange: NSRange)

Sets the location for the first glyph in the specified range.

func setNotShownAttribute(Bool, forGlyphAt: Int)

Sets the visibility of the glyph at the specified index.

