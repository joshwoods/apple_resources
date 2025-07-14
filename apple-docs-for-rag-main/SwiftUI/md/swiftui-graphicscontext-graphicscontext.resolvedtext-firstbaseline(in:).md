

- SwiftUI
- GraphicsContext
- GraphicsContext.ResolvedText
-  firstBaseline(in:) 

Instance Method

# firstBaseline(in:)

Gets the distance from the first line’s ascender to its baseline.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func firstBaseline(in size: CGSize) -> CGFloat
```

## See Also

### Getting the text properties

func lastBaseline(in: CGSize) -> CGFloat

Gets the distance from the first line’s ascender to the last line’s baseline.

func measure(in: CGSize) -> CGSize

Measures the size of the resolved text for a given area into which the text should be placed.

var shading: GraphicsContext.Shading

The shading to fill uncolored text regions with.

