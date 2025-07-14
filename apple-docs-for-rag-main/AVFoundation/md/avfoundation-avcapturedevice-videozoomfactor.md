

- AVFoundation
- AVCaptureDevice
-  videoZoomFactor 

Instance Property

# videoZoomFactor

A value that controls the cropping and enlargement of images captured by the device.

iOS 7.0+iPadOS 7.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var videoZoomFactor: CGFloat { get set }
```

## Mentioned in 

Enhancing your app experience with the Camera Control

## Discussion

This value is a multiplier. For example, a value of `2.0` doubles the size of an image’s subject (and halves the field of view). Allowed values range from `1.0` (full field of view) to the value of the active format’s videoMaxZoomFactor property. Setting the value of this property jumps immediately to the new zoom factor. For a smooth transition, use the ramp(toVideoZoomFactor:withRate:) method.

The device achieves a zoom effect by cropping around the center of the image captured by the sensor. At low zoom factors, the cropped images is equal to or larger than the output size. At higher zoom factors, the device must scale the cropped image up to the output size, resulting in a loss of image quality. The active format’s videoZoomFactorUpscaleThreshold property indicates the factors at which upscaling occurs.

Before changing the value of this property, you must call lockForConfiguration() to acquire exclusive access to the device’s configuration properties. Otherwise, setting the value of this property raises an exception. When you finish configuring the device, call unlockForConfiguration() to release the lock and allow other devices to configure the settings.

## See Also

### Adjusting Zoom

func ramp(toVideoZoomFactor: CGFloat, withRate: Float)

Begins a smooth transition from the current zoom factor to another.

func cancelVideoZoomRamp()

Smoothly ends a zoom transition in progress.

