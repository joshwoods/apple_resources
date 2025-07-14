

- AppKit
- NSTypesetter
-  characterRange(forGlyphRange:actualGlyphRange:) 

Instance Method

# characterRange(forGlyphRange:actualGlyphRange:)

Returns the range for the characters in the receiver’s text store that are mapped to the specified glyphs.

macOS

``` source
func characterRange(
    forGlyphRange glyphRange: NSRange,
    actualGlyphRange: NSRangePointer?
) -> NSRange
```

## Parameters 

`glyphRange`  

The range of glyphs.

`actualGlyphRange`  

On return, the range of all glyphs mapped to the characters in the receiver’s text store. May be `NULL`.

## Return Value

The range for the characters in the receiver’s text store that are mapped to the glyphs in `glyphRange`.

## Discussion

A subclass can override this method to interact with custom glyph storage.

## See Also

### Interfacing with Glyph Storage

func glyphRange(forCharacterRange: NSRange, actualCharacterRange: NSRangePointer?) -> NSRange

Returns the range for the glyphs mapped to the characters of the text store in the specified range.

func setAttachmentSize(NSSize, forGlyphRange: NSRange)

Sets the size the specified glyphs (assumed to be attachments) will be asked to draw themselves at.

func setBidiLevels(UnsafePointer&lt;UInt8>!, forGlyphRange: NSRange)

Sets the direction of the specified glyphs for bidirectional text.

func setDrawsOutsideLineFragment(Bool, forGlyphRange: NSRange)

Sets whether the specified glyphs exceed the bounds of the line fragment in which they are laid out.

func setLineFragmentRect(NSRect, forGlyphRange: NSRange, usedRect: NSRect, baselineOffset: CGFloat)

Sets the line fragment rectangle where the specified glyphs are laid out.

func setLocation(NSPoint, withAdvancements: UnsafePointer&lt;CGFloat>!, forStartOfGlyphRange: NSRange)

Sets the location where the specified glyphs are laid out.

func setNotShownAttribute(Bool, forGlyphRange: NSRange)

Sets whether the specified glyphs are not shown.

