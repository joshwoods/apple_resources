

- ARKit
-  ARSCNPlaneGeometry 

Class

# ARSCNPlaneGeometry

A SceneKit representation of the 2D shape of a plane, for use with plane detection results in an AR session.

iOS 11.3+iPadOS 11.3+Mac Catalyst 13.1+

``` source
class ARSCNPlaneGeometry
```

## Overview

ARSCNPlaneGeometry is a subclass of SCNGeometry that wraps the mesh data provided by the ARPlaneGeometry class. You can use ARSCNPlaneGeometry to visualize the plane shape estimates provided by ARKit in a SceneKit view.

Important

ARSCNPlaneGeometry is available only in SceneKit views or renderers that use Metal. This class is not supported for OpenGL-based SceneKit rendering.

As your AR session continues to run, ARKit provides refined estimates of a detected plane’s 2D shape. Use the update(from:) method to incorporate those refinements into the plane’s SceneKit representation.

## Topics

### Creating a Geometry

convenience init?(device: any MTLDevice)

Creates a SceneKit plane geometry for rendering with the specified Metal device object.

### Updating the Geometry

func update(from: ARPlaneGeometry)

Reshapes the SceneKit geometry to match the specified plane mesh.

## Relationships

### Inherits From

- SCNGeometry

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- SCNAnimatable
- SCNBoundingVolume
- SCNShadable

## See Also

### Geometry

var geometry: ARPlaneGeometry

A coarse triangle mesh representing the general shape of the detected plane.

class ARPlaneGeometry

A 3D mesh describing the shape of a detected plane in world-tracking AR sessions.

