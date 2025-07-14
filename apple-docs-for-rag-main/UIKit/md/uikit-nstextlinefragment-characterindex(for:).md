

- UIKit
- NSTextLineFragment
-  characterIndex(for:) 

Instance Method

# characterIndex(for:)

Returns character index for a point inside the line fragment coordinate system.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
func characterIndex(for point: CGPoint) -> Int
```

## Parameters 

`point`  

The distance is from the upstream edge.

## Return Value

An integer that represents the character index at `point`.

## See Also

### Finding specific text

func fractionOfDistanceThroughGlyph(for: CGPoint) -> CGFloat

Returns character index for a point inside the line fragment coordinate system.

func locationForCharacter(at: Int) -> CGPoint

Returns the location of the character at the specified index.

