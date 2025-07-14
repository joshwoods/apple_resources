

- RealityKit
- ModelSortGroup
-  depthPass 

Instance Property

# depthPass

A depth pass that controls when the renderer draws the depth of model entities in the group relative to their color.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
var depthPass: ModelSortGroup.DepthPass? { get }
```

## Discussion

You can tell the renderer to draw the depth and color together by setting the value to `nil`.

