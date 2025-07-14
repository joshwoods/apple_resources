

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.SystemPressureState
- AVCaptureDevice.SystemPressureState.Level
-  serious 

Type Property

# serious

A level that indicates that system pressure is highly elevated.

iOS 11.1+iPadOS 11.1+Mac Catalyst 14.0+tvOS 17.0+visionOS 1.0+

``` source
static let serious: AVCaptureDevice.SystemPressureState.Level
```

## Discussion

System pressures may impact capture performance. Consider limiting the frame rate until system pressure state improves.

## See Also

### System Pressure Levels

static let nominal: AVCaptureDevice.SystemPressureState.Level

A level that indicates the system pressure is normal and not under pressure.

static let fair: AVCaptureDevice.SystemPressureState.Level

A level that indicates that system pressure is slightly elevated.

static let critical: AVCaptureDevice.SystemPressureState.Level

System pressure is critically elevated.

static let shutdown: AVCaptureDevice.SystemPressureState.Level

System pressure is beyond critical, so the capture system has shut down.

