

- UIKit
- NSTextLineFragment
-  locationForCharacter(at:) 

Instance Method

# locationForCharacter(at:)

Returns the location of the character at the specified index.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
func locationForCharacter(at index: Int) -> CGPoint
```

## Parameters 

`index`  

An integer that represents the position in the text.

## Return Value

A CGPoint that’s on the upstream edge of the glyph. It’s in the coordinate system relative to the line fragment origin.

## See Also

### Finding specific text

func characterIndex(for: CGPoint) -> Int

Returns character index for a point inside the line fragment coordinate system.

func fractionOfDistanceThroughGlyph(for: CGPoint) -> CGFloat

Returns character index for a point inside the line fragment coordinate system.

