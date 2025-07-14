

- SwiftUI
- GraphicsContext
- GraphicsContext.ResolvedImage
-  shading 

Instance Property

# shading

An optional shading to fill the image with.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var shading: GraphicsContext.Shading?
```

## Discussion

The value of this property defaults to foreground for template images, and to `nil` otherwise.

## See Also

### Getting the image properties

var size: CGSize

The size of the image.

let baseline: CGFloat

The distance from the top of the image to its baseline.

