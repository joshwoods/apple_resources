

- ARKit
- CameraFrame
- CameraFrame.Sample
- CameraFrame.Sample.Parameters
-  extrinsics 

Instance Property

# extrinsics

The camera extrinsics.

visionOS 2.0+

``` source
var extrinsics: simd_float4x4 { get }
```

## See Also

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

var intrinsics: simd_float3x3

var midExposureTimestamp: TimeInterval

The mid exposure timestamp.

