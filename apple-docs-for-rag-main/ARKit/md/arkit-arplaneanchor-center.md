

- ARKit
- ARPlaneAnchor
-  center 

Instance Property

# center

The center point of the plane relative to its anchor position.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
var center: simd_float3 { get }
```

## Discussion

When ARKit first detects a plane, the resulting ARPlaneAnchor object has a center value of `(0,0,0)`, indicating that the translation portion of the anchor’s transform value locates the plane’s center point.

As scene analysis and plane detection continues, ARKit may determine that a previously detected plane anchor is part of a larger real-world surface, increasing the extent width and length values. The plane’s new boundaries may not be symmetric around its initial position, so the center point changes relative to the anchor’s (unchanged) transform matrix.

Although the type of this property is vector_float3, a plane anchor is always two-dimensional, and is always positioned in only the x and z directions relative to its transform position. (That is, the y-component of this vector is always zero.)

## See Also

### Dimensions

var planeExtent: ARPlaneExtent

The estimated width, length, and y-axis rotation of the detected plane.

class ARPlaneExtent

The size and y-axis rotation of a detected plane.

var extent: simd_float3

The estimated width and length of the detected plane.

Deprecated

