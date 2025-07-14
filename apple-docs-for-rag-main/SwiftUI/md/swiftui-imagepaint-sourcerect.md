

- SwiftUI
- ImagePaint
-  sourceRect 

Instance Property

# sourceRect

A unit-space rectangle defining how much of the source image to draw.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var sourceRect: CGRect
```

## Discussion

The results are undefined if this rectangle selects areas outside the `[0, 1]` range in either axis.

## See Also

### Configuring the image paint style

var image: Image

The image to be drawn.

var scale: CGFloat

A scale factor applied to the image while being drawn.

