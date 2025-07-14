

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.SystemPressureState
- AVCaptureDevice.SystemPressureState.Level
-  critical 

Type Property

# critical

System pressure is critically elevated.

iOS 11.1+iPadOS 11.1+Mac Catalyst 14.0+tvOS 17.0+visionOS 1.0+

``` source
static let critical: AVCaptureDevice.SystemPressureState.Level
```

## Discussion

Capture quality and performance are significantly impacted. Reduce the frame rate until system pressure state improves.

## See Also

### System Pressure Levels

static let nominal: AVCaptureDevice.SystemPressureState.Level

A level that indicates the system pressure is normal and not under pressure.

static let fair: AVCaptureDevice.SystemPressureState.Level

A level that indicates that system pressure is slightly elevated.

static let serious: AVCaptureDevice.SystemPressureState.Level

A level that indicates that system pressure is highly elevated.

static let shutdown: AVCaptureDevice.SystemPressureState.Level

System pressure is beyond critical, so the capture system has shut down.

