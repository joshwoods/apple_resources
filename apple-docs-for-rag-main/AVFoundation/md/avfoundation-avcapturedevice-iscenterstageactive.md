

- AVFoundation
- AVCaptureDevice
-  isCenterStageActive 

Instance Property

# isCenterStageActive

A Boolean value that indicates whether Center Stage is active on a device.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 12.3+tvOS 17.0+

``` source
var isCenterStageActive: Bool { get }
```

## Discussion

When Center Stage is active, the camera automatically pans, tightens, or widens the field of view as it requires to keep people optimally framed. If an app or a user enables Center Stage, this property value is true if the device supports the feature in its current configuration.

The system imposes the following restrictions on a device when Center Stage is active:

- It limits the range of values the device supports for its minAvailableVideoZoomFactor and maxAvailableVideoZoomFactor properties to those of the active capture format’s videoMinZoomFactorForCenterStage and videoMaxZoomFactorForCenterStage, respectively.

- It limits the activeVideoMinFrameDuration and activeVideoMaxFrameDuration to the value set by the active capture format’s videoFrameRateRangeForCenterStage property.

The system deactivates Center Stage in the following cases:

- You enable depth data delivery on a capture output, such as AVCaptureDepthDataOutput or AVCapturePhotoOutput.

- The device supports geometric distortion correction, but you haven’t enabled it by setting the value of isGeometricDistortionCorrectionEnabled to true.

This property is key-value observable.

## See Also

### Configuring Center Stage

class var isCenterStageEnabled: Bool

A Boolean value that indicates whether a user or an app enabled Center Stage on a device.

var centerStageRectOfInterest: CGRect

The effective region within the output pixel buffer to perform Center Stage framing.

class var centerStageControlMode: AVCaptureDevice.CenterStageControlMode

A value that indicates the current mode of Center Stage control.

enum CenterStageControlMode

Constants that indicate the current Center Stage control mode.

