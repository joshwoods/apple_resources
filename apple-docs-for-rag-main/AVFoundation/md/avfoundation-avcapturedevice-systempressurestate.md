

- AVFoundation
- AVCaptureDevice
-  systemPressureState 

Instance Property

# systemPressureState

A value that indicates the capture device’s current system pressure state.

iOS 11.1+iPadOS 11.1+Mac Catalyst 14.0+tvOS 17.0+

``` source
var systemPressureState: AVCaptureDevice.SystemPressureState { get }
```

## Discussion

This property indicates whether the capture device is currently in an elevated system pressure condition. When system pressure reaches a shutdown state, the capture device can’t continue to provide input, and the capture session becomes interrupted until the pressured state abates.

You can effectively mitigate system pressure by lowering the device’s activeVideoMinFrameDuration in response to changes in the system pressure state. Implement frame rate throttling to bring system pressure down if your capture use case can tolerate a reduced frame rate.

## See Also

### Monitoring System Pressure

class SystemPressureState

An object that provides information about OS and hardware status affecting capture system performance and availability.

let AVCaptureSessionInterruptionSystemPressureStateKey: String

A key to retrieve a state value that indicates the system pressure level and contributing factors that caused the interruption.

