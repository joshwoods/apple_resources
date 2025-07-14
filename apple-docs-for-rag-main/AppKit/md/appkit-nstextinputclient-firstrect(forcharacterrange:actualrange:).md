

- AppKit
- NSTextInputClient
-  firstRect(forCharacterRange:actualRange:) 

Instance Method

# firstRect(forCharacterRange:actualRange:)

Returns the first logical boundary rectangle for characters in the given range.

macOS

``` source
func firstRect(
    forCharacterRange range: NSRange,
    actualRange: NSRangePointer?
) -> NSRect
```

**Required**

## Parameters 

`range`  

The character range whose boundary rectangle is returned.

`actualRange`  

If non-`NULL`, contains the character range corresponding to the returned area if it was adjusted, for example, to a grapheme cluster boundary or characters in the first line fragment.

## Return Value

The boundary rectangle for the given range of characters, in screen coordinates. The rectangle’s `size` value can be negative if the text flows to the left.

## Discussion

If `aRange` spans multiple lines of text in the text view, the rectangle returned is the one surrounding the characters in the first line. In that case `actualRange` contains the range covered by the first rect, so you can query all line fragments by invoking this method repeatedly. If the length of `aRange` is 0 (as it would be if there is nothing selected at the insertion point), the rectangle coincides with the insertion point, and its width is 0.

## See Also

### Getting character coordinates

func characterIndex(for: NSPoint) -> Int

Returns the index of the character whose bounding rectangle includes the given point.

**Required**

func baselineDeltaForCharacter(at: Int) -> CGFloat

Returns the baseline position of a given character relative to the origin of rectangle returned by firstRect(forCharacterRange:actualRange:).

func drawsVerticallyForCharacter(at: Int) -> Bool

Informs the text input management system whether the protocol-conforming client renders the character at the given index vertically.

func fractionOfDistanceThroughGlyph(for: NSPoint) -> CGFloat

Returns the fraction of the distance from the left side of the character to the right side that a given point lies.

