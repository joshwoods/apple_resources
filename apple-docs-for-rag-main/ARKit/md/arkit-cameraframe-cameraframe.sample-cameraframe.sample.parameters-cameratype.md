

- ARKit
- CameraFrame
- CameraFrame.Sample
- CameraFrame.Sample.Parameters
-  cameraType 

Instance Property

# cameraType

visionOS 2.0+

``` source
var cameraType: CameraFrameProvider.CameraType { get }
```

## See Also

### Getting frame parameters

var cameraPosition: CameraFrameProvider.CameraPosition

The camera position.

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

