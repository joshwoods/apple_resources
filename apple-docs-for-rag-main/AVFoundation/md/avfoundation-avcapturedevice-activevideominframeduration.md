

- AVFoundation
- AVCaptureDevice
-  activeVideoMinFrameDuration 

Instance Property

# activeVideoMinFrameDuration

The currently active minimum frame duration.

iOS 7.0+iPadOS 7.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 1.0+

``` source
var activeVideoMinFrameDuration: CMTime { get set }
```

## Discussion

A device’s minimum frame duration is the reciprocal of its maximum frame rate. You can set the value of this property to limit the maximum frame rate during a capture session. The capture device automatically chooses a default minimum frame duration based on its active format. After changing the value of this property, you can return to the default minimum frame duration by setting this property’s value to invalid. Choosing a new preset for the capture session also resets this property to its default value.

Attempting to set this property to a value not found in the active format’s videoSupportedFrameRateRanges array raises an exception (invalidArgumentException).

Important

Before changing the value of this property, you must call lockForConfiguration() to acquire exclusive access to the device’s configuration properties. Otherwise, setting the value of this property raises an exception. When you’re done configuring the device, call unlockForConfiguration() to release the lock.

This property value is key-value observable.

## See Also

### Configuring Frame Durations

var activeVideoMaxFrameDuration: CMTime

The currently active maximum frame duration.

var activeDepthDataMinFrameDuration: CMTime

The minimum frame duration of depth data.

