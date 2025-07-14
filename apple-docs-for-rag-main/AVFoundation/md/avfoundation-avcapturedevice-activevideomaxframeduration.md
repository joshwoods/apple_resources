

- AVFoundation
- AVCaptureDevice
-  activeVideoMaxFrameDuration 

Instance Property

# activeVideoMaxFrameDuration

The currently active maximum frame duration.

iOS 7.0+iPadOS 7.0+Mac Catalyst 14.0+macOS 10.9+tvOS 17.0+visionOS 1.0+

``` source
var activeVideoMaxFrameDuration: CMTime { get set }
```

## Discussion

A device’s maximum frame duration is the reciprocal of its minimum frame rate. You can set the value of this property to limit the minimum frame rate during a capture session. The capture device automatically chooses a default maximum frame duration based on its active format. After changing the value of this property, you can return to the default maximum frame duration by setting this property’s value to invalid. Choosing a new preset for the capture session also resets this property to its default value.

Attempting to set this property to a value not found in the active format’s videoSupportedFrameRateRanges array raises an exception (invalidArgumentException).

Important

Before changing the value of this property, you must call lockForConfiguration() to acquire exclusive access to the device’s configuration properties. Otherwise, setting the value of this property raises an exception. When you’re done configuring the device, call unlockForConfiguration() to release the lock.

This property value is key-value observable.

## See Also

### Configuring Frame Durations

var activeVideoMinFrameDuration: CMTime

The currently active minimum frame duration.

var activeDepthDataMinFrameDuration: CMTime

The minimum frame duration of depth data.

