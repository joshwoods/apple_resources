

- AppKit
- NSTypesetter
-  setLocation(\_:withAdvancements:forStartOfGlyphRange:) 

Instance Method

# setLocation(\_:withAdvancements:forStartOfGlyphRange:)

Sets the location where the specified glyphs are laid out.

macOS

``` source
func setLocation(
    _ location: NSPoint,
    withAdvancements advancements: UnsafePointer!,
    forStartOfGlyphRange glyphRange: NSRange
)
```

## Parameters 

`location`  

The location where the glyphs in `glyphRange` are laid out. The x-coordinate of `location` is expressed relative to the line fragment rectangle origin, and the y-coordinate is expressed relative to the baseline previously specified by setLineFragmentRect(_:forGlyphRange:usedRect:baselineOffset:).

`advancements`  

The nominal glyph advance width specified in the font metric information.

`glyphRange`  

The range of glyphs whose layout location is being set. This series of glyphs can be displayed with a single PostScript `show` operation (a nominal range).

## Discussion

Setting the location for a series of glyphs implies that the glyphs preceding it can’t be included in a single `show` operation.

Before setting the location for a glyph range, you must specify line fragment rectangle with setLineFragmentRect(_:forGlyphRange:usedRect:baselineOffset:).

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

func setNotShownAttribute(Bool, forGlyphRange: NSRange)

Sets whether the specified glyphs are not shown.

