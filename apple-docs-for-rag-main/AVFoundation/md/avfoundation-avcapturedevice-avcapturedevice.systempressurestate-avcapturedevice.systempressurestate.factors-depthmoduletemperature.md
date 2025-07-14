

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.SystemPressureState
- AVCaptureDevice.SystemPressureState.Factors
-  depthModuleTemperature 

Type Property

# depthModuleTemperature

The module capturing depth information is operating at an elevated temperature.

iOS 11.1+iPadOS 11.1+Mac Catalyst 14.0+tvOS 17.0+visionOS 1.0+

``` source
static var depthModuleTemperature: AVCaptureDevice.SystemPressureState.Factors { get }
```

## Discussion

As system pressure increases, depth quality may become degraded. To reduce system pressure from this factor, reduce depth capture frame rate.

This factor applies only to builtInTrueDepthCamera devices.

## See Also

### System Pressure Factors

static var systemTemperature: AVCaptureDevice.SystemPressureState.Factors

The entire system is under elevated thermal load.

static var peakPower: AVCaptureDevice.SystemPressureState.Factors

The system’s peak power requirements exceed the battery’s current capacity.

static var cameraTemperature: AVCaptureDevice.SystemPressureState.Factors

The camera module is operating at an elevated temperature.

