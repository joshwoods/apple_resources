

- ARKit
- CameraFrame
- CameraFrame.Sample
- CameraFrame.Sample.Parameters
-  midExposureTimestamp 

Instance Property

# midExposureTimestamp

The mid exposure timestamp.

visionOS 2.0+

``` source
var midExposureTimestamp: TimeInterval { get }
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

var extrinsics: simd_float4x4

The camera extrinsics.

var intrinsics: simd_float3x3

