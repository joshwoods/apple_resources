

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.SystemPressureState
- AVCaptureDevice.SystemPressureState.Level
-  shutdown 

Type Property

# shutdown

System pressure is beyond critical, so the capture system has shut down.

iOS 11.1+iPadOS 11.1+Mac Catalyst 14.0+tvOS 17.0+visionOS 1.0+

``` source
static let shutdown: AVCaptureDevice.SystemPressureState.Level
```

## Discussion

When system pressure reaches this level, the capture system automatically shuts down, causing a session interruption. Use the AVCaptureSessionInterruptionSystemPressureStateKey in the interruption notification’s userInfo dictionary to find details about the system pressure factors causing the interruption.

## See Also

### System Pressure Levels

static let nominal: AVCaptureDevice.SystemPressureState.Level

A level that indicates the system pressure is normal and not under pressure.

static let fair: AVCaptureDevice.SystemPressureState.Level

A level that indicates that system pressure is slightly elevated.

static let serious: AVCaptureDevice.SystemPressureState.Level

A level that indicates that system pressure is highly elevated.

static let critical: AVCaptureDevice.SystemPressureState.Level

System pressure is critically elevated.

