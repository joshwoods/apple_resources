

- AVFoundation
- AVCaptureDevice
-  iso 

Instance Property

# iso

The current exposure ISO value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var iso: Float { get }
```

## Discussion

This property controls the sensor’s sensitivity to light by applying a gain value to the signal. This value is between the active format’s minISO and maxISO values. Higher values result in noisier images.

To set the ISO, call the setExposureModeCustom(duration:iso:completionHandler:) method.

This property is key-value observable.

## See Also

### Configuring Exposure Manually

var exposureDuration: CMTime

The length of time over which exposure takes place.

var activeMaxExposureDuration: CMTime

The maximum exposure duration, in seconds, defined in the autoexposure algorithm.

var lensAperture: Float

The size of the lens diaphragm.

func setExposureModeCustom(duration: CMTime, iso: Float, completionHandler: ((CMTime) -> Void)?)

Sets the exposure mode to a custom state, and locks exposure duration and ISO at explicit values.

