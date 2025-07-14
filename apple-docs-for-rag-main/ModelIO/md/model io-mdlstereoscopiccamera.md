

- Model I/O
-  MDLStereoscopicCamera 

Class

# MDLStereoscopicCamera

A point of view for rendering a stereoscopic display of a 3D scene.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class MDLStereoscopicCamera
```

## Overview

This class provides properties related to rendering the scene from two slightly different perspectives to simulate binocular vision. For general and optical properties of a camera, see the superclass MDLCamera.

## Topics

### Modeling Stereoscopic Imaging

var interPupillaryDistance: Float

The distance, in millimeters, between the stereoscopic camera’s two viewpoints.

var overlap: Float

The amount, as a fraction of image width, by which the images from the camera’s two viewpoints overlap.

var leftVergence: Float

The angle, in degrees, at which the camera’s left viewpoint faces toward a central focal point.

var rightVergence: Float

The angle, in degrees, at which the camera’s right viewpoint faces toward a central focal point.

### Generating View and Projection Matrices

var leftViewMatrix: matrix_float4x4

The transformation matrix that determines the position and orientation of the camera’s left viewpoint relative to a scene.

var leftProjectionMatrix: matrix_float4x4

The transformation matrix that determines the extent of a scene visible to the camera’s left viewpoint.

var rightViewMatrix: matrix_float4x4

The transformation matrix that determines the position and orientation of the camera’s right viewpoint relative to a scene.

var rightProjectionMatrix: matrix_float4x4

The transformation matrix that determines the extent of a scene visible to the camera’s right viewpoint.

## Relationships

### Inherits From

- MDLCamera

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- MDLNamed
- NSObjectProtocol

## See Also

### Cameras

class MDLCamera

A point of view for rendering a 3D scene, along with a set of parameters describing an intended appearance for rendering.

