

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.SystemPressureState
- AVCaptureDevice.SystemPressureState.Factors
-  peakPower 

Type Property

# peakPower

The system’s peak power requirements exceed the battery’s current capacity.

iOS 11.1+iPadOS 11.1+Mac Catalyst 14.0+tvOS 17.0+visionOS 1.0+

``` source
static var peakPower: AVCaptureDevice.SystemPressureState.Factors { get }
```

## Discussion

Devices with chemically aged batteries are less able to respond to rapid increases in total power usage (CPU and GPU usage, I/O, camera systems, radios, etc). When a device detects such conditions, the system may limit capture sperformance to prevent an unexpected device shutdown.

## See Also

### System Pressure Factors

static var systemTemperature: AVCaptureDevice.SystemPressureState.Factors

The entire system is under elevated thermal load.

static var depthModuleTemperature: AVCaptureDevice.SystemPressureState.Factors

The module capturing depth information is operating at an elevated temperature.

static var cameraTemperature: AVCaptureDevice.SystemPressureState.Factors

The camera module is operating at an elevated temperature.

