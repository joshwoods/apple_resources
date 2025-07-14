

- AppKit
- NSTypesetter
-  setLineFragmentRect(\_:forGlyphRange:usedRect:baselineOffset:) 

Instance Method

# setLineFragmentRect(\_:forGlyphRange:usedRect:baselineOffset:)

Sets the line fragment rectangle where the specified glyphs are laid out.

macOS

``` source
func setLineFragmentRect(
    _ fragmentRect: NSRect,
    forGlyphRange glyphRange: NSRange,
    usedRect: NSRect,
    baselineOffset: CGFloat
)
```

## Parameters 

`fragmentRect`  

The line fragment rectangle where the glyphs in `glyphRange` are laid out.

`glyphRange`  

The range of the specified glyphs.

`usedRect`  

The portion of `fragmentRect`, in the NSTextContainer object’s coordinate system, that actually contains glyphs or other marks that are drawn (including the text container’s line fragment padding). The `usedRect` must be equal to or contained within `fragmentRect`.

`baselineOffset`  

The vertical distance in pixels from the line fragment origin to the baseline on which the glyphs align.

## Discussion

The exact positions of the glyphs must be set after the line fragment rectangle with `setLocation:forStartOfGlyphRange:`.

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

func setLocation(NSPoint, withAdvancements: UnsafePointer&lt;CGFloat>!, forStartOfGlyphRange: NSRange)

Sets the location where the specified glyphs are laid out.

func setNotShownAttribute(Bool, forGlyphRange: NSRange)

Sets whether the specified glyphs are not shown.

