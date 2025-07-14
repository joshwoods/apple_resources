

- ARKit
- CameraFrame
- CameraFrame.Sample
- CameraFrame.Sample.Parameters
-  colorTemperature 

Instance Property

# colorTemperature

The white balance correlated color temperature in kelvin.

visionOS 2.0+

``` source
var colorTemperature: Int { get }
```

## See Also

### Getting frame parameters

var cameraPosition: CameraFrameProvider.CameraPosition

The camera position.

var cameraType: CameraFrameProvider.CameraType

var captureTimestamp: TimeInterval

The capture timestamp.

var exposureDuration: CFTimeInterval

The camera frame exposure duration in seconds.

var extrinsics: simd_float4x4

The camera extrinsics.

var intrinsics: simd_float3x3

var midExposureTimestamp: TimeInterval

The mid exposure timestamp.

