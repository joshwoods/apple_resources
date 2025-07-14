

- RealityKit
- MeshResource
- MeshResource.GenerateTextOptions
-  containerFrame 

Instance Property

# containerFrame

The size in points of the frame where the text is laid out.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var containerFrame: CGRect?
```

## Discussion

The points are scaled at a ratio of 72 points per meter.

The container frame has the same origin as the local coordinate system.

Note

Use a value of `nil` to denote an arbitrarily large frame.

