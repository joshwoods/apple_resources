

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.SystemPressureState
- AVCaptureDevice.SystemPressureState.Level
-  nominal 

Type Property

# nominal

A level that indicates the system pressure is normal and not under pressure.

iOS 11.1+iPadOS 11.1+Mac Catalyst 14.0+tvOS 17.0+visionOS 1.0+

``` source
static let nominal: AVCaptureDevice.SystemPressureState.Level
```

## See Also

### System Pressure Levels

static let fair: AVCaptureDevice.SystemPressureState.Level

A level that indicates that system pressure is slightly elevated.

static let serious: AVCaptureDevice.SystemPressureState.Level

A level that indicates that system pressure is highly elevated.

static let critical: AVCaptureDevice.SystemPressureState.Level

System pressure is critically elevated.

static let shutdown: AVCaptureDevice.SystemPressureState.Level

System pressure is beyond critical, so the capture system has shut down.

