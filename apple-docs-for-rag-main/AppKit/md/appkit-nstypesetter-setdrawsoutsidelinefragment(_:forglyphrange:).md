

- AppKit
- NSTypesetter
-  setDrawsOutsideLineFragment(\_:forGlyphRange:) 

Instance Method

# setDrawsOutsideLineFragment(\_:forGlyphRange:)

Sets whether the specified glyphs exceed the bounds of the line fragment in which they are laid out.

macOS

``` source
func setDrawsOutsideLineFragment(
    _ flag: Bool,
    forGlyphRange glyphRange: NSRange
)
```

## Parameters 

`flag`  

true if the glyphs in `glyphRange` exceed the bounds of the line fragment in which they are laid out, false otherwise.

`glyphRange`  

The range of the glyphs in question.

## Discussion

This can happen when text is set at a fixed line height. For example, if the user specifies a fixed line height of 12 points and sets the font size to 24 points, the glyphs will exceed their layout rectangles.

A subclass can override this method to interact with custom glyph storage.

## See Also

### Interfacing with Glyph Storage

func characterRange(forGlyphRange: NSRange, actualGlyphRange: NSRangePointer?) -> NSRange

Returns the range for the characters in the receiver’s text store that are mapped to the specified glyphs.

func glyphRange(forCharacterRange: NSRange, actualCharacterRange: NSRangePointer?) -> NSRange

Returns the range for the glyphs mapped to the characters of the text store in the specified range.

func setAttachmentSize(NSSize, forGlyphRange: NSRange)

Sets the size the specified glyphs (assumed to be attachments) will be asked to draw themselves at.

func setBidiLevels(UnsafePointer&lt;UInt8>!, forGlyphRange: NSRange)

Sets the direction of the specified glyphs for bidirectional text.

func setLineFragmentRect(NSRect, forGlyphRange: NSRange, usedRect: NSRect, baselineOffset: CGFloat)

Sets the line fragment rectangle where the specified glyphs are laid out.

func setLocation(NSPoint, withAdvancements: UnsafePointer&lt;CGFloat>!, forStartOfGlyphRange: NSRange)

Sets the location where the specified glyphs are laid out.

func setNotShownAttribute(Bool, forGlyphRange: NSRange)

Sets whether the specified glyphs are not shown.

