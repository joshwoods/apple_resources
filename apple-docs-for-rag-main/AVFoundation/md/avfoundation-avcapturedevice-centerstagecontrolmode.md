

- AVFoundation
- AVCaptureDevice
-  centerStageControlMode 

Type Property

# centerStageControlMode

A value that indicates the current mode of Center Stage control.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 12.3+tvOS 17.0+

``` source
class var centerStageControlMode: AVCaptureDevice.CenterStageControlMode { get set }
```

## Discussion

See Control Modes for details on choosing an appropriate control mode.

## See Also

### Configuring Center Stage

var isCenterStageActive: Bool

A Boolean value that indicates whether Center Stage is active on a device.

class var isCenterStageEnabled: Bool

A Boolean value that indicates whether a user or an app enabled Center Stage on a device.

var centerStageRectOfInterest: CGRect

The effective region within the output pixel buffer to perform Center Stage framing.

enum CenterStageControlMode

Constants that indicate the current Center Stage control mode.

