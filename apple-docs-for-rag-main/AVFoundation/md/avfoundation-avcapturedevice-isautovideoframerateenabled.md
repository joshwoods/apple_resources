

- AVFoundation
- AVCaptureDevice
-  isAutoVideoFrameRateEnabled 

Instance Property

# isAutoVideoFrameRateEnabled

A Boolean value that indicates whether the capture device performs automatic video frame rate adjustments.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+

``` source
var isAutoVideoFrameRateEnabled: Bool { get set }
```

## Discussion

You can enable this property on a device when its active format’s isAutoVideoFrameRateSupported property is true. When enabled, a capture device automatically adjusts the active frame rate based on light level. Under low light conditions, it decreases the frame rate to properly expose the scene. For formats with a maximum frame rate of 30 fps, the frame rate switches between 30-24. For formats with a maximum frame rate of 60 fps, the frame rate switches between 60-30-24.

Important

After enabling automatic frame rate adjustments, attempting to set a device’s activeVideoMinFrameDuration or activeVideoMaxFrameDuration throws an exception.

Changing the device’s active format resets this property to its default value of false.

