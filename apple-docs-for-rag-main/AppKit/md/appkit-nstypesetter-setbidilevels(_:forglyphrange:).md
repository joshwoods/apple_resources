

- AppKit
- NSTypesetter
-  setBidiLevels(\_:forGlyphRange:) 

Instance Method

# setBidiLevels(\_:forGlyphRange:)

Sets the direction of the specified glyphs for bidirectional text.

macOS

``` source
func setBidiLevels(
    _ levels: UnsafePointer!,
    forGlyphRange glyphRange: NSRange
)
```

## Parameters 

`levels`  

Values in `levels` can range from 0 to 61 as defined by Unicode Standard Annex \#9.

`glyphRange`  

The range of glyphs for which the bidirectional text levels are desired.

## Discussion

A subclass can override this method to interact with custom glyph storage.

## See Also

### Interfacing with Glyph Storage

func characterRange(forGlyphRange: NSRange, actualGlyphRange: NSRangePointer?) -> NSRange

Returns the range for the characters in the receiver’s text store that are mapped to the specified glyphs.

func glyphRange(forCharacterRange: NSRange, actualCharacterRange: NSRangePointer?) -> NSRange

Returns the range for the glyphs mapped to the characters of the text store in the specified range.

func setAttachmentSize(NSSize, forGlyphRange: NSRange)

Sets the size the specified glyphs (assumed to be attachments) will be asked to draw themselves at.

func setDrawsOutsideLineFragment(Bool, forGlyphRange: NSRange)

Sets whether the specified glyphs exceed the bounds of the line fragment in which they are laid out.

func setLineFragmentRect(NSRect, forGlyphRange: NSRange, usedRect: NSRect, baselineOffset: CGFloat)

Sets the line fragment rectangle where the specified glyphs are laid out.

func setLocation(NSPoint, withAdvancements: UnsafePointer&lt;CGFloat>!, forStartOfGlyphRange: NSRange)

Sets the location where the specified glyphs are laid out.

func setNotShownAttribute(Bool, forGlyphRange: NSRange)

Sets whether the specified glyphs are not shown.

