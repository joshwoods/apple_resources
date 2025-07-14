

- RealityKit
- TextComponent
-  cornerRadius 

Instance Property

# cornerRadius

The corner radius of the text mesh.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
var cornerRadius: Float
```

## Discussion

The corner geometry is based on a circular shape and is not a continuous corner. Text components use the CoreGraphics coordinate space: The origin is at the upper left of the canvas and positive values extend down and to the right.

