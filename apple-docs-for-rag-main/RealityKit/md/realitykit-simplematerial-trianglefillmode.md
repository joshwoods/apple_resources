

- RealityKit
- SimpleMaterial
-  triangleFillMode 

Instance Property

# triangleFillMode

The object that controls how RealityKit draws triangles.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
var triangleFillMode: SimpleMaterial.TriangleFillMode { get set }
```

## Discussion

A value of MaterialParameterTypes.TriangleFillMode.fill causes RealityKit to draw triangles normally, while a value of MaterialParameterTypes.TriangleFillMode.lines turns on wireframe rendering.

