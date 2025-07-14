

- ARKit
-  ARCamera 

Class

# ARCamera

Information about the camera position and imaging characteristics for a given frame.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
class ARCamera
```

## Mentioned in 

Managing Session Life Cycle and Tracking Quality

Understanding World Tracking

## Overview

You get camera information from the camera property of each ARFrame ARKit delivers.

## Topics

### Handling Tracking Status

var trackingState: ARCamera.TrackingState

The general quality of position tracking available when the camera captured a frame.

enum TrackingState

Values for position tracking quality, with possible causes when tracking quality is limited.

### Examining Camera Geometry

var transform: simd_float4x4

The position and orientation of the camera in world coordinate space.

var eulerAngles: simd_float3

The orientation of the camera, expressed as roll, pitch, and yaw values.

### Examining Imaging Parameters

var imageResolution: CGSize

The width and height, in pixels, of the captured camera image.

var intrinsics: simd_float3x3

A matrix that converts between the 2D camera plane and 3D world coordinate space.

### Applying Camera Geometry

var projectionMatrix: simd_float4x4

A transform matrix appropriate for rendering 3D content to match the image captured by the camera.

func projectionMatrix(for: UIInterfaceOrientation, viewportSize: CGSize, zNear: CGFloat, zFar: CGFloat) -> simd_float4x4

Returns a transform matrix appropriate for rendering 3D content to match the image captured by the camera, using the specified parameters.

func viewMatrix(for: UIInterfaceOrientation) -> simd_float4x4

Returns a transform matrix for converting from world space to camera space.

func projectPoint(simd_float3, orientation: UIInterfaceOrientation, viewportSize: CGSize) -> CGPoint

Returns the projection of a point from the 3D world space detected by ARKit into the 2D space of a view rendering the scene.

func unprojectPoint(CGPoint, ontoPlane: simd_float4x4, orientation: UIInterfaceOrientation, viewportSize: CGSize) -> simd_float3?

Returns the projection of a point from the 2D space of a view rendering the scene onto a plane in the 3D world space detected by ARKit.

### Applying Motion Blur

var exposureDuration: TimeInterval

A value you use to effect motion blur when rendering your app’s virtual content.

### Applying Post-Processed Lighting

var exposureOffset: Float

A value you supply to your custom renderer to light your scene.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol
- Sendable

