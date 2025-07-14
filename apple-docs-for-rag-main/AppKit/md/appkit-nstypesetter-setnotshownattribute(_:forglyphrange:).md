

- AppKit
- NSTypesetter
-  setNotShownAttribute(\_:forGlyphRange:) 

Instance Method

# setNotShownAttribute(\_:forGlyphRange:)

Sets whether the specified glyphs are not shown.

macOS

``` source
func setNotShownAttribute(
    _ flag: Bool,
    forGlyphRange glyphRange: NSRange
)
```

## Parameters 

`flag`  

true if the glyphs in `glyphRange` are not shown, false if they are shown.

`glyphRange`  

The range of glyphs in question.

## Discussion

For example, a tab or newline character doesn’t leave any marks; it just indicates where following glyphs are laid out.

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

func setDrawsOutsideLineFragment(Bool, forGlyphRange: NSRange)

Sets whether the specified glyphs exceed the bounds of the line fragment in which they are laid out.

func setLineFragmentRect(NSRect, forGlyphRange: NSRange, usedRect: NSRect, baselineOffset: CGFloat)

Sets the line fragment rectangle where the specified glyphs are laid out.

func setLocation(NSPoint, withAdvancements: UnsafePointer&lt;CGFloat>!, forStartOfGlyphRange: NSRange)

Sets the location where the specified glyphs are laid out.

