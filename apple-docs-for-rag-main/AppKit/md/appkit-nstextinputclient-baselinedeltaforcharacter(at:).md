

- AppKit
- NSTextInputClient
-  baselineDeltaForCharacter(at:) 

Instance Method

# baselineDeltaForCharacter(at:)

Returns the baseline position of a given character relative to the origin of rectangle returned by firstRect(forCharacterRange:actualRange:).

macOS 10.0+

``` source
optional func baselineDeltaForCharacter(at anIndex: Int) -> CGFloat
```

## Parameters 

`anIndex`  

Index of the character whose baseline is tested.

## Return Value

The vertical distance, in points, between the baseline of the character at `anIndex` and the rectangle origin.

## Discussion

Implementation of this method is optional. This information allows the caller to determine finer-grained character positioning within the text storage of the text view adopting `NSTextInputClient`.

## See Also

### Getting character coordinates

func characterIndex(for: NSPoint) -> Int

Returns the index of the character whose bounding rectangle includes the given point.

**Required**

func firstRect(forCharacterRange: NSRange, actualRange: NSRangePointer?) -> NSRect

Returns the first logical boundary rectangle for characters in the given range.

**Required**

func drawsVerticallyForCharacter(at: Int) -> Bool

Informs the text input management system whether the protocol-conforming client renders the character at the given index vertically.

func fractionOfDistanceThroughGlyph(for: NSPoint) -> CGFloat

Returns the fraction of the distance from the left side of the character to the right side that a given point lies.

