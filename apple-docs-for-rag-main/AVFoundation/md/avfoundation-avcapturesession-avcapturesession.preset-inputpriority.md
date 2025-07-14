

- AVFoundation
- AVCaptureSession
- AVCaptureSession.Preset
-  inputPriority 

Type Property

# inputPriority

A preset that doesn’t specify audio and video output settings for a capture session.

iOS 7.0+iPadOS 7.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
static let inputPriority: AVCaptureSession.Preset
```

## Discussion

To enable capture settings not supported by any session presets (such as high frame rate), change the value of the activeFormat property on the appropriate capture device. When you change the device’s format, the session preset automatically changes to this value, indicating that the AVCaptureSession object has relinquished responsibility for configuring its inputs and outputs. (Instead, the capture device’s active format dictates the quality of service level provided at the outputs). To return to automatic configuration, use the session’s sessionPreset property to choose another preset.

