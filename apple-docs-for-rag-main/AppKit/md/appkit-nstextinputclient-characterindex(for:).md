

- AppKit
- NSTextInputClient
-  characterIndex(for:) 

Instance Method

# characterIndex(for:)

Returns the index of the character whose bounding rectangle includes the given point.

macOS

``` source
func characterIndex(for point: NSPoint) -> Int
```

**Required**

## Parameters 

`point`  

The point to test, in screen coordinates.

## Return Value

The character index, measured from the start of the receiver’s text storage, of the character containing the given point. Returns `NSNotFound` if the cursor is not within a character’s bounding rectangle.

## See Also

### Getting character coordinates

func firstRect(forCharacterRange: NSRange, actualRange: NSRangePointer?) -> NSRect

Returns the first logical boundary rectangle for characters in the given range.

**Required**

func baselineDeltaForCharacter(at: Int) -> CGFloat

Returns the baseline position of a given character relative to the origin of rectangle returned by firstRect(forCharacterRange:actualRange:).

func drawsVerticallyForCharacter(at: Int) -> Bool

Informs the text input management system whether the protocol-conforming client renders the character at the given index vertically.

func fractionOfDistanceThroughGlyph(for: NSPoint) -> CGFloat

Returns the fraction of the distance from the left side of the character to the right side that a given point lies.

