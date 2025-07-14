

- RealityKit
- BoundingBox
-  boundingRadius 

Instance Property

# boundingRadius

The radius of a bounding sphere that encompasses the bounding box.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
var boundingRadius: Float { get }
```

## Discussion

This value is 0 if the box is empty.

## See Also

### Getting the box characteristics

var max: SIMD3&lt;Float>

The position of the maximum corner of the box.

var min: SIMD3&lt;Float>

The position of the minimum corner of the box.

var center: SIMD3&lt;Float>

The center of the bounding box.

var extents: SIMD3&lt;Float>

The extents of the bounding box.

