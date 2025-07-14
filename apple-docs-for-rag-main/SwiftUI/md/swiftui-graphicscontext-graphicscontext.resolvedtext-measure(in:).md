

- SwiftUI
- GraphicsContext
- GraphicsContext.ResolvedText
-  measure(in:) 

Instance Method

# measure(in:)

Measures the size of the resolved text for a given area into which the text should be placed.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func measure(in size: CGSize) -> CGSize
```

## Parameters 

`size`  

The area to place the Text view in.

## See Also

### Getting the text properties

func firstBaseline(in: CGSize) -> CGFloat

Gets the distance from the first line’s ascender to its baseline.

func lastBaseline(in: CGSize) -> CGFloat

Gets the distance from the first line’s ascender to the last line’s baseline.

var shading: GraphicsContext.Shading

The shading to fill uncolored text regions with.

