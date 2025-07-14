

- ARKit
- CameraFrame
- CameraFrame.Sample
- CameraFrame.Sample.Parameters
-  exposureDuration 

Instance Property

# exposureDuration

The camera frame exposure duration in seconds.

visionOS 2.0+

``` source
var exposureDuration: CFTimeInterval { get }
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

var extrinsics: simd_float4x4

The camera extrinsics.

var intrinsics: simd_float3x3

var midExposureTimestamp: TimeInterval

The mid exposure timestamp.

