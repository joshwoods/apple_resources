

- AppKit
- NSTextInputClient
-  drawsVerticallyForCharacter(at:) 

Instance Method

# drawsVerticallyForCharacter(at:)

Informs the text input management system whether the protocol-conforming client renders the character at the given index vertically.

macOS 10.6+

``` source
optional func drawsVerticallyForCharacter(at charIndex: Int) -> Bool
```

## Parameters 

`charIndex`  

The index of the character to test.

## Return Value

true if the character is rendered vertically; otherwise false.

## See Also

### Getting character coordinates

func characterIndex(for: NSPoint) -> Int

Returns the index of the character whose bounding rectangle includes the given point.

**Required**

func firstRect(forCharacterRange: NSRange, actualRange: NSRangePointer?) -> NSRect

Returns the first logical boundary rectangle for characters in the given range.

**Required**

func baselineDeltaForCharacter(at: Int) -> CGFloat

Returns the baseline position of a given character relative to the origin of rectangle returned by firstRect(forCharacterRange:actualRange:).

func fractionOfDistanceThroughGlyph(for: NSPoint) -> CGFloat

Returns the fraction of the distance from the left side of the character to the right side that a given point lies.

