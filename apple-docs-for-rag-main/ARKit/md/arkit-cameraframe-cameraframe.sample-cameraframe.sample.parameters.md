

- ARKit
- CameraFrame
- CameraFrame.Sample
-  CameraFrame.Sample.Parameters 

Structure

# CameraFrame.Sample.Parameters

A frame’s parameters, such as the camera type, intrinsics, timestamps, exposure, and so on.

visionOS 2.0+

``` source
struct Parameters
```

## Topics

### Getting frame parameters

var cameraPosition: CameraFrameProvider.CameraPosition

The camera position.

var cameraType: CameraFrameProvider.CameraType

var captureTimestamp: TimeInterval

The capture timestamp.

var colorTemperature: Int

The white balance correlated color temperature in kelvin.

var exposureDuration: CFTimeInterval

The camera frame exposure duration in seconds.

var extrinsics: simd_float4x4

The camera extrinsics.

var intrinsics: simd_float3x3

var midExposureTimestamp: TimeInterval

The mid exposure timestamp.

### Instance Properties

var description: String

A textual representation of these camera frame parameters.

## Relationships

### Conforms To

- CustomStringConvertible
- Equatable
- Sendable

## See Also

### Inspecting camera frame samples

var parameters: CameraFrame.Sample.Parameters

The frame’s parameters.

var pixelBuffer: CVPixelBuffer

