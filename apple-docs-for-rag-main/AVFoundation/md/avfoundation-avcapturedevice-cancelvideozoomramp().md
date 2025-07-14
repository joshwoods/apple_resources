

- AVFoundation
- AVCaptureDevice
-  cancelVideoZoomRamp() 

Instance Method

# cancelVideoZoomRamp()

Smoothly ends a zoom transition in progress.

iOS 7.0+iPadOS 7.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
func cancelVideoZoomRamp()
```

## Discussion

Calling this method is equivalent to calling ramp(toVideoZoomFactor:withRate:) with a rate of zero. If a zoom transition is in progress, the transition slows to a stop (instead of stopping abruptly).

Before calling this method, you must call lockForConfiguration() to acquire exclusive access to the device’s configuration properties. If you don’t, calling this method raises an exception. When you finish configuring the device, call unlockForConfiguration() to release the lock and allow other devices to configure the settings.

## See Also

### Adjusting Zoom

var videoZoomFactor: CGFloat

A value that controls the cropping and enlargement of images captured by the device.

func ramp(toVideoZoomFactor: CGFloat, withRate: Float)

Begins a smooth transition from the current zoom factor to another.

