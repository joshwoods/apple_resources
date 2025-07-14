

- AVFoundation
-  AVCaptureSessionInterruptionSystemPressureStateKey 

Global Variable

# AVCaptureSessionInterruptionSystemPressureStateKey

A key to retrieve a state value that indicates the system pressure level and contributing factors that caused the interruption.

iOS 11.1+iPadOS 11.1+Mac Catalyst 14.0+tvOS 17.0+visionOS 1.0+

``` source
let AVCaptureSessionInterruptionSystemPressureStateKey: String
```

## Discussion

If an interruption occurs and the value of AVCaptureSessionInterruptionReasonKey equals AVCaptureSession.InterruptionReason.videoDeviceNotAvailableDueToSystemPressure, the userInfo dictionary for the notification contains this key and a corresponding AVCaptureDevice.SystemPressureState value.

## See Also

### Monitoring System Pressure

var systemPressureState: AVCaptureDevice.SystemPressureState

A value that indicates the capture device’s current system pressure state.

class SystemPressureState

An object that provides information about OS and hardware status affecting capture system performance and availability.

