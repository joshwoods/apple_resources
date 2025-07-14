

- ARKit
-  ARFaceAnchor 

Class

# ARFaceAnchor

An anchor for a unique face that is visible in the front-facing camera.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
class ARFaceAnchor
```

## Mentioned in 

Understanding World Tracking

## Overview

The session automatically adds to its list of anchors an ARFaceAnchor object when it detects a unique face in the front camera feed.

When you track faces using ARFaceTrackingConfiguration, ARKit can track multiple faces simultaneously.

Alternatively, you can enable face tracking with a world tracking configuration by setting .

### Tracking Face Position and Orientation

The inherited transform property describes the face’s current position and orientation in world coordinates; that is, in a coordinate space relative to that specified by the worldAlignment property of the session configuration. Use this transform matrix to position virtual content you want to “attach” to the face in your AR scene.

This transform matrix creates a face coordinates system for positioning other elements relative to the face. Units of face coordinate space are in meters, with the origin centered behind the face as indicated in the figure below.

The coordinate system is right-handed—the positive x direction points to the viewer’s right (that is, the face’s own left), the positive y direction points up (relative to the face itself, not to the world), and the positive z direction points outward from the face (toward the viewer).

### Using Face Topology

The geometry property provides an ARFaceGeometry object representing detailed topology for the face, which conforms a generic face model to match the dimensions, shape, and current expression of the detected face.

You can use this model as the basis for overlaying content that follows the shape of the user’s face—for example, to apply virtual makeup or tattoos. You can also use this model to create *occlusion geometry*—a 3D model that doesn’t render any visible content (allowing the camera image to show through), but that obstructs the camera’s view of other virtual content in the scene.

### Tracking Facial Expressions

The blendShapes property provides a high-level model of the current facial expression, described via a series of many named coefficients that represent the movement of specific facial features relative to their neutral configurations. You can use blend shape coefficients to animate 2D or 3D content, such as a character or avatar, in ways that follow the user’s facial expressions.

## Topics

### Using Face Geometry

var geometry: ARFaceGeometry

A coarse triangle mesh representing the topology of the detected face.

### Using Blend Shapes

var blendShapes: [ARFaceAnchor.BlendShapeLocation : NSNumber]

A dictionary of named coefficients representing the detected facial expression in terms of the movement of specific facial features.

struct BlendShapeLocation

Identifiers for specific facial features, for use with coefficients describing the relative movements of those features.

### Tracking Eye Movement

var leftEyeTransform: simd_float4x4

A transform matrix indicating the position and orientation of the face’s left eye.

var rightEyeTransform: simd_float4x4

A transform matrix indicating the position and orientation of the face’s right eye.

var lookAtPoint: simd_float3

A position in face coordinate space estimating the direction of the face’s gaze.

## Relationships

### Inherits From

- ARAnchor

### Conforms To

- ARAnchorCopying
- ARTrackable
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

### Face Tracking

Tracking and visualizing faces

Detect faces in a front-camera AR experience, overlay virtual content, and animate facial expressions in real-time.

Combining user face-tracking and world tracking

Track the user’s face in an app that displays an AR experience with the rear camera.

