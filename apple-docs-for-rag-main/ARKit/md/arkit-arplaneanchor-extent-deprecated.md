

- ARKit
- ARPlaneAnchor
-  extent Deprecated

Instance Property

# extent

The estimated width and length of the detected plane.

iOS 11.0–16.0DeprecatediPadOS 11.0–16.0DeprecatedMac Catalyst 13.1–16.0Deprecated

``` source
var extent: simd_float3 { get }
```

## Discussion

Warning

In iOS 16, use planeExtent instead.

The framework sets the x and z components to the width and length of the plane, respectively. The y-component is unused, with a constant value of `0`.

## See Also

### Dimensions

var center: simd_float3

The center point of the plane relative to its anchor position.

var planeExtent: ARPlaneExtent

The estimated width, length, and y-axis rotation of the detected plane.

class ARPlaneExtent

The size and y-axis rotation of a detected plane.

