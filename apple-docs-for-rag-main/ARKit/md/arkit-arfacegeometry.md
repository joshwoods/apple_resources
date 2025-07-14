

- ARKit
-  ARFaceGeometry 

Class

# ARFaceGeometry

A 3D mesh describing face topology for use in face-tracking AR sessions.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
class ARFaceGeometry
```

## Overview

This class provides a general model for the detailed topology of a face, in the form of a 3D mesh appropriate for use with various rendering technologies or for exporting 3D assets. (For a quick way to visualize a face geometry using SceneKit, see the ARSCNFaceGeometry class.)

When you obtain a face geometry from an ARFaceAnchor object in a face-tracking AR session, the model conforms to match the dimensions, shape, and current expression of the detected face. You can also create a face mesh using a dictionary of named blend shape coefficients, which provides a detailed, but more efficient, description of the face’s current expression.

In an AR session, you can use this model as the basis for overlaying content that follows the shape of the user’s face—for example, to apply virtual makeup or tattoos. You can also use this model to create occlusion geometry, which hides other virtual content behind the 3D shape of the detected face in the camera image.

Note

Face mesh topology is constant across ARFaceGeometry instances. That is, the values of the vertexCount, textureCoordinateCount, and triangleCount properties never change, the triangleIndices buffer always describes the same arrangement of vertices, and the textureCoordinates buffer always maps the same vertex indices to the same texture coordinates.

Only the vertices buffer changes between face meshes provided by an AR session, indicating the change in vertex positions as ARKit adapts the mesh to the shape and expression of the user’s face.

## Topics

### Accessing Mesh Data

var vertices: [simd_float3]

An array of vertex positions for each point in the face mesh.

var textureCoordinates: [vector_float2]

An array of texture coordinate values for each point in the face mesh.

var triangleCount: Int

The number of triangles described by the triangleIndices buffer.

var triangleIndices: [Int16]

An array of indices describing the triangle mesh formed by the face geometry’s vertex data.

### Creating a Mesh from Blend Shapes

init?(blendShapes: [ARFaceAnchor.BlendShapeLocation : NSNumber])

Creates a face geometry matching the facial expression described in the specified dictionary.

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
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Face Data

Tracking and visualizing faces

Detect faces in a front-camera AR experience, overlay virtual content, and animate facial expressions in real-time.

Combining user face-tracking and world tracking

Track the user’s face in an app that displays an AR experience with the rear camera.

class ARSCNFaceGeometry

A SceneKit representation of face topology for use with face information that an AR session provides.

