

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.SystemPressureState
-  level 

Instance Property

# level

The overall level of performance constraints on the capture system.

iOS 11.1+iPadOS 11.1+Mac Catalyst 14.0+tvOS 17.0+visionOS 1.0+

``` source
var level: AVCaptureDevice.SystemPressureState.Level { get }
```

## Discussion

Several aspects of OS and hardware status affect capture system performance and availability (see AVCaptureDevice.SystemPressureState.Factors). The overall system pressure level represents the most critical of underlying factors.

## See Also

### Overall Level

struct Level

A structure that defines system pressure state levels.

