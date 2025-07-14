

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.SystemPressureState
- AVCaptureDevice.SystemPressureState.Level
-  fair 

Type Property

# fair

A level that indicates that system pressure is slightly elevated.

iOS 11.1+iPadOS 11.1+Mac Catalyst 14.0+tvOS 17.0+visionOS 1.0+

``` source
static let fair: AVCaptureDevice.SystemPressureState.Level
```

## See Also

### System Pressure Levels

static let nominal: AVCaptureDevice.SystemPressureState.Level

A level that indicates the system pressure is normal and not under pressure.

static let serious: AVCaptureDevice.SystemPressureState.Level

A level that indicates that system pressure is highly elevated.

static let critical: AVCaptureDevice.SystemPressureState.Level

System pressure is critically elevated.

static let shutdown: AVCaptureDevice.SystemPressureState.Level

System pressure is beyond critical, so the capture system has shut down.

