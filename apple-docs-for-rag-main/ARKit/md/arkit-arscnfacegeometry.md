

- ARKit
-  ARSCNFaceGeometry 

Class

# ARSCNFaceGeometry

A SceneKit representation of face topology for use with face information that an AR session provides.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
class ARSCNFaceGeometry
```

## Overview

This class is a subclass of SCNGeometry that wraps the mesh data provided by the ARFaceGeometry class. You can use ARSCNFaceGeometry to quickly and easily visualize face topology and facial expressions provided by ARKit in a SceneKit view.

Important

ARSCNFaceGeometry is available only in SceneKit views or renderers that use Metal. This class is not supported for OpenGL-based SceneKit rendering.

Face mesh topology is constant for the lifetime of an ARSCNFaceGeometry object. That is, the geometry’s single SCNGeometryElement object always describes the same arrangement of vertices, and the texcoord geometry source always maps the same vertices to the same texture coordinates.

When you modify the geometry with the update(from:) method, only the contents of the vertex geometry source change, indicating the difference in vertex positions as ARKit adapts the mesh to the shape and expression of the user’s face.

## Topics

### Creating a Geometry

convenience init?(device: any MTLDevice)

Creates a SceneKit face geometry for rendering with the specified Metal device object.

convenience init?(device: any MTLDevice, fillMesh: Bool)

Creates a SceneKit face geometry, optionally filling in gaps in the mesh for the eyes and mouth.

### Updating the Geometry

func update(from: ARFaceGeometry)

Deforms the SceneKit geometry to match the specified face mesh.

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

### Face Data

Tracking and visualizing faces

Detect faces in a front-camera AR experience, overlay virtual content, and animate facial expressions in real-time.

Combining user face-tracking and world tracking

Track the user’s face in an app that displays an AR experience with the rear camera.

class ARFaceGeometry

A 3D mesh describing face topology for use in face-tracking AR sessions.

