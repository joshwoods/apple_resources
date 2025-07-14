

- AVFoundation
- AVCaptureDeviceInput
-  videoMinFrameDurationOverride 

Instance Property

# videoMinFrameDurationOverride

A time value that acts as a modifier to a capture device’s active video minimum frame duration.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var videoMinFrameDurationOverride: CMTime { get set }
```

## Discussion

A capture device’s activeVideoMinFrameDuration property is the reciprocal of its active maximum frame rate. To limit the maximum frame rate of the capture device, you may set activeVideoMinFrameDuration to a value supported by the device’s activeFormat. Changes you make to the device’s activeVideoMinFrameDuration value take effect immediately without disrupting preview. Therefore, AVCaptureSession must always allocate sufficient resources to allow the device to run at its active format’s maximum frame rate.

If you wish to use a particular device format but run it only at lower frame rates (for instance, only run a 1080p240 fps format at a maximum frame rate of 60), set the input’s videoMinFrameDurationOverride property to the reciprocal of the maximum frame rate you intend to use before starting the session (or within a beginConfiguration() / commitConfiguration() block while running the session).

This property’s default value is invalid. When you remove a device input from a session and then add it back, this property reverts to its default value.

## See Also

### Configuring video properties

var unifiedAutoExposureDefaultsEnabled: Bool

A Boolean value that indicates whether the input enables unified auto-exposure defaults.

