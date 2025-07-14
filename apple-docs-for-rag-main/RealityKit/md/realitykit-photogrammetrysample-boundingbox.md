

- RealityKit
- PhotogrammetrySample
-  boundingBox 

Instance Property

# boundingBox

The bounding box of the scene or object being captured, represented as the transform of a unit cube centered at the origin into an oriented box in the session’s world coordinate system. The transform can be factored as an SRT into the scale (axis length), orientation (rotation), and center (translation) using `Transform(matrix:)`.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
var boundingBox: simd_float4x4? { get }
```

