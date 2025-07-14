

- AVFoundation
-  AVCameraCalibrationData 

Class

# AVCameraCalibrationData

Information about the camera characteristics used to capture images and depth data.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class AVCameraCalibrationData
```

## Overview

Information about the calibration of a camera—such as its pixel focal length, principal point, and lens distortion characteristics—helps to determine the geometric relationships between the camera device and the images it captures. You can use this information to accurately render visual effects into images produced by a camera or perform computer vision tasks such as correcting images for geometric distortions.

## Topics

### Mapping Pixels to Scene Geometry

var intrinsicMatrix: matrix_float3x3

A matrix that relates a camera’s internal properties to an ideal pinhole-camera model.

var intrinsicMatrixReferenceDimensions: CGSize

The image dimensions to which the camera’s intrinsic matrix values are relative.

var extrinsicMatrix: matrix_float4x3

A matrix relating a camera’s position and orientation to a world or scene coordinate system.

var pixelSize: Float

The size, in millimeters, of one image pixel.

### Correcting for Lens Distortion

var lensDistortionLookupTable: Data?

A map of floating-point values describing radial distortions imparted by the camera lens, for use in rectifying camera images.

var inverseLensDistortionLookupTable: Data?

A map of floating-point values describing radial distortions for use in reapplying camera geometry to a rectified image.

var lensDistortionCenter: CGPoint

The offset of the distortion center of the camera lens from the top-left corner of the image.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Depth data capture

Capturing Photos with Depth

Get a depth map with a photo to create effects like the system camera’s Portrait mode (on compatible devices).

Creating Auxiliary Depth Data Manually

Generate a depth image and attach it to your own image.

Capturing depth using the LiDAR camera

Access the LiDAR camera on supporting devices to capture precise depth data.

AVCamFilter: Applying Filters to a Capture Stream

Render a capture stream with rose-colored filtering and depth effects.

Streaming Depth Data from the TrueDepth Camera

Visualize depth data in 2D and 3D from the TrueDepth camera.

Enhancing Live Video by Leveraging TrueDepth Camera Data

Apply your own background to a live capture feed streamed from the front-facing TrueDepth camera.

class AVCaptureDepthDataOutput

A capture output that records scene depth information on compatible camera devices.

class AVDepthData

A container for per-pixel distance or disparity information captured by compatible camera devices.

