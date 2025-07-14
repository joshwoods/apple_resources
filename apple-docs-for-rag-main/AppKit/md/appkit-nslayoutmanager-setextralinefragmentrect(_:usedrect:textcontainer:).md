

- AppKit
- NSLayoutManager
-  setExtraLineFragmentRect(\_:usedRect:textContainer:) 

Instance Method

# setExtraLineFragmentRect(\_:usedRect:textContainer:)

Sets the bounds and container for the extra line fragment.

macOS 10.7+

``` source
func setExtraLineFragmentRect(
    _ fragmentRect: NSRect,
    usedRect: NSRect,
    textContainer container: NSTextContainer
)
```

## Parameters 

`fragmentRect`  

The rectangle to set.

`usedRect`  

Indicates where the insertion point is drawn.

`container`  

The text container where the rectangle is to be laid out.

## Discussion

The extra line fragment is used when the text backing ends with a hard line break or when the text backing is totally empty, to define the extra line which needs to be displayed at the end of the text. If the text backing is not empty and does not end with a hard line break, this should be set to NSZeroRect and `nil`.

Line fragment rectangles and line fragment used rectangles are always in container coordinates.

This method is used by the layout mechanism and should be invoked only during typesetting, in almost all cases only by the typesetter. For example, a custom typesetter might invoke it.

## See Also

### Setting layout information

func setAttachmentSize(NSSize, forGlyphRange: NSRange)

Sets the size to use when drawing a glyph that represents an attachment.

func setDrawsOutsideLineFragment(Bool, forGlyphAt: Int)

Indicates whether the specified glyph exceeds the bounds of the line fragment for its layout.

func setLineFragmentRect(NSRect, forGlyphRange: NSRange, usedRect: NSRect)

Associates the line fragment bounds for the specified range of glyphs.

func setLocation(NSPoint, forStartOfGlyphRange: NSRange)

Sets the location for the first glyph in the specified range.

func setNotShownAttribute(Bool, forGlyphAt: Int)

Sets the visibility of the glyph at the specified index.

