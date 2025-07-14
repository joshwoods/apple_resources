

- AppKit
- NSTextLineFragment
-  fractionOfDistanceThroughGlyph(for:) 

Instance Method

# fractionOfDistanceThroughGlyph(for:)

Returns character index for a point inside the line fragment coordinate system.

macOS 12.0+

``` source
func fractionOfDistanceThroughGlyph(for point: CGPoint) -> CGFloat
```

## Parameters 

`point`  

A CGPoint that represents the point inside the line fragment.

## Return Value

The fraction of distance from the upstream edge.

## See Also

### Finding specific text

func characterIndex(for: CGPoint) -> Int

Returns character index for a point inside the line fragment coordinate system.

func locationForCharacter(at: Int) -> CGPoint

Returns the location of the character at the specified index.

