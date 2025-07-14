

- AppKit
- NSLayoutManager
-  textStorage(\_:edited:range:changeInLength:invalidatedRange:) Deprecated

Instance Method

# textStorage(\_:edited:range:changeInLength:invalidatedRange:)

Invalidates glyph and layout information for a portion of the text in the given text storage object.

macOS 10.0–10.11Deprecated

``` source
func textStorage(
    _ str: NSTextStorage,
    edited editedMask: Int = [],
    range newCharRange: NSRange,
    changeInLength delta: Int,
    invalidatedRange invalidatedCharRange: NSRange
)
```

Deprecated

Use processEditing(for:edited:range:changeInLength:invalidatedRange:) instead.

## Parameters 

`str`  

The text storage whose information is invalidated.

`editedMask`  

Specifies the nature of the changes. Its value is made by combining with the C bitwise OR operator the constants described in “Change notifications” in NSTextStorage (editedAttributes and editedCharacters).

`newCharRange`  

Indicates the extent of characters resulting from the edits.

`delta`  

If the `NSTextStorageEditedCharacters` bit of `mask` is set, gives the number of characters added to or removed from the original range (otherwise its value is irrelevant).

`invalidatedCharRange`  

Represents the range of characters affected after attributes have been fixed. Is either equal to `newCharRange` or larger. For example, deleting a paragraph separator character invalidates the layout information for all characters in the paragraphs that precede and follow the separator.

## Discussion

This message is sent from the `NSTextStorage`object’s processEditing() method to indicate that its characters or attributes have changed. This method invalidates glyphs and layout for the affected characters.

For example, after replacing “The” with “Several” to produce the string “Several files couldn’t be saved”, `newCharRange` is {0, 7} and `delta` is 4. The receiver uses this information to update its character-to-glyph mapping and to update the selection range based on the change.

The textStorage(_:edited:range:changeInLength:invalidatedRange:) messages are sent in a series to each `NSLayoutManager` object associated with the text storage object, so the layout managers receiving them shouldn’t edit `aTextStorage` while this method is executing. If one of them does, the `newCharRange`, `delta`, and `invalidatedCharRange` arguments are incorrect for all following layout managers that receive the message.

## See Also

### Methods

func showCGGlyphs(UnsafePointer&lt;CGGlyph>, positions: UnsafePointer&lt;NSPoint>, count: Int, font: NSFont, matrix: AffineTransform, attributes: [NSAttributedString.Key : Any], in: NSGraphicsContext)

Renders the glyphs at the specified positions, using the specified attributes.

Deprecated

func invalidateGlyphs(onLayoutInvalidationForGlyphRange: NSRange)

Specifies explicitly when portions of the glyph stream depend on layout.

Deprecated

func invalidateLayout(forCharacterRange: NSRange, isSoft: Bool, actualCharacterRange: NSRangePointer?)

Invalidates the layout information for the glyphs mapped to the given range of characters.

Deprecated

func insertGlyph(NSGlyph, atGlyphIndex: Int, characterIndex: Int)

Inserts a single glyph into the glyph stream at the given index and maps it to the character at the given character index.

Deprecated

func insertGlyphs(UnsafePointer&lt;NSGlyph>, length: Int, forStartingGlyphAt: Int, characterIndex: Int)

Inserts the given glyphs into the glyph cache at the given index and maps them to characters beginning at the given character index.

Deprecated

func glyph(at: Int) -> NSGlyph

Returns the glyph at the specified index.

Deprecated

func glyph(at: Int, isValidIndex: UnsafeMutablePointer&lt;ObjCBool>?) -> NSGlyph

Returns the glyph at a specified index, and optionally returns a flag indicating whether the requested index is valid.

Deprecated

func replaceGlyph(at: Int, withGlyph: NSGlyph)

Replaces the glyph at the given index with a new glyph.

Deprecated

func getGlyphs(UnsafeMutablePointer&lt;NSGlyph>?, range: NSRange) -> Int

Fills the passed-in buffer with a sequence of glyphs.

Deprecated

func getGlyphs(in: NSRange, glyphs: UnsafeMutablePointer&lt;NSGlyph>?, characterIndexes: UnsafeMutablePointer&lt;Int>?, glyphInscriptions: UnsafeMutablePointer&lt;NSGlyphInscription>?, elasticBits: UnsafeMutablePointer&lt;ObjCBool>?) -> Int

Returns the glyphs and information needed to perform layout for the given glyph range.

Deprecated

func getGlyphs(in: NSRange, glyphs: UnsafeMutablePointer&lt;NSGlyph>?, characterIndexes: UnsafeMutablePointer&lt;Int>?, glyphInscriptions: UnsafeMutablePointer&lt;NSGlyphInscription>?, elasticBits: UnsafeMutablePointer&lt;ObjCBool>?, bidiLevels: UnsafeMutablePointer&lt;UInt8>?) -> Int

Returns the glyphs and information needed to perform layout for the given glyph range.

Deprecated

func deleteGlyphs(in: NSRange)

Deletes the glyphs in the given range from the receiver’s glyph store.

Deprecated

func setCharacterIndex(Int, forGlyphAt: Int)

Sets the index of the character corresponding to the glyph at the given glyph index.

Deprecated

func intAttribute(Int, forGlyphAt: Int) -> Int

Returns the value of the attribute identified by the given attribute tag for the glyph at the given index.

Deprecated

func setIntAttribute(Int, value: Int, forGlyphAt: Int)

Sets a custom attribute value for a given glyph.

Deprecated

