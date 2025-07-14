

- ARKit
-  ARPlaneExtent 

Class

# ARPlaneExtent

The size and y-axis rotation of a detected plane.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
class ARPlaneExtent
```

## Overview

A plane anchor (ARPlaneAnchor) describes its size and orientation on the y-axis using the planeExtent property of this type.

At runtime, ARKit continually updates the anchor’s width and height as the framework refines its knowledge of the plane’s shape in the environment.

Similarly, as the session runs, the framework may update the plane’s y-rotation to better fit its rectangular area in the environment. In iOS 15 and earlier, the framework rotates the plane anchor according to that angle. In iOS 16, the framework doesn’t rotate the anchor automatically and its transform matrix remains unchanged. Instead, the framework exposes the angle rotationOnYAxis that you apply to any plane extent geometry in your app.

Important

Apps that run on iOS 16 with a deployment target less than iOS 16 preserve the prior y-axis rotation behavior.

### Size and Rotate an Entity to a Plane’s Extent

The following code defines a RealityKit entity sized to the plane extent’s width and height. The helper function also applies the extent’s suggested y-axis rotation by setting its transform `yaw` value to rotationOnYAxis.

```
func createPlane(for planeAnchor: ARPlaneAnchor, material: Material) -> ModelEntity {

    // Get the plane's extent.
    let extent = planeAnchor.planeExtent

    // Create a model entity sized to the plane's extent.
    let planeEntity = ModelEntity(mesh: .generatePlane (width: extent.width, depth: extent.height),
        materials: [material])

    // Orient the entity according to the extent's y-axis rotation.
    planeEntity.transform = Transform(pitch: 0, yaw: extent.rotationOnYAxis, roll: 0)

    // Center the entity on the plane.
    planeEntity.transform.translation = planeAnchor.center

    return planeEntity
}
```

## Topics

### Inspecting Plane Size

var width: Float

The estimated width of the plane.

var height: Float

The estimated height of the plane.

### Inspecting Plane Y-Rotation

var rotationOnYAxis: Float

A radian value that indicates a plane’s y-axis orientation.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Dimensions

var center: simd_float3

The center point of the plane relative to its anchor position.

var planeExtent: ARPlaneExtent

The estimated width, length, and y-axis rotation of the detected plane.

var extent: simd_float3

The estimated width and length of the detected plane.

Deprecated

