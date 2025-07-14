

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.SystemPressureState
- AVCaptureDevice.SystemPressureState.Factors
-  cameraTemperature 

Type Property

# cameraTemperature

The camera module is operating at an elevated temperature.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+

``` source
static var cameraTemperature: AVCaptureDevice.SystemPressureState.Factors { get }
```

## See Also

### System Pressure Factors

static var systemTemperature: AVCaptureDevice.SystemPressureState.Factors

The entire system is under elevated thermal load.

static var peakPower: AVCaptureDevice.SystemPressureState.Factors

The system’s peak power requirements exceed the battery’s current capacity.

static var depthModuleTemperature: AVCaptureDevice.SystemPressureState.Factors

The module capturing depth information is operating at an elevated temperature.

