

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.SystemPressureState
- AVCaptureDevice.SystemPressureState.Factors
-  systemTemperature 

Type Property

# systemTemperature

The entire system is under elevated thermal load.

iOS 11.1+iPadOS 11.1+Mac Catalyst 14.0+tvOS 17.0+visionOS 1.0+

``` source
static var systemTemperature: AVCaptureDevice.SystemPressureState.Factors { get }
```

## See Also

### System Pressure Factors

static var peakPower: AVCaptureDevice.SystemPressureState.Factors

The system’s peak power requirements exceed the battery’s current capacity.

static var depthModuleTemperature: AVCaptureDevice.SystemPressureState.Factors

The module capturing depth information is operating at an elevated temperature.

static var cameraTemperature: AVCaptureDevice.SystemPressureState.Factors

The camera module is operating at an elevated temperature.

