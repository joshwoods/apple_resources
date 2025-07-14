

- AVFoundation
- AVCaptureDevice
-  exposureDuration 

Instance Property

# exposureDuration

The length of time over which exposure takes place.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var exposureDuration: CMTime { get }
```

## Discussion

The exposure duration is between the active format’s minExposureDuration and maxExposureDuration.

To set the exposure duration, call the setExposureModeCustom(duration:iso:completionHandler:) method.

This property is key-value observable.

## See Also

### Configuring Exposure Manually

var activeMaxExposureDuration: CMTime

The maximum exposure duration, in seconds, defined in the autoexposure algorithm.

var iso: Float

The current exposure ISO value.

var lensAperture: Float

The size of the lens diaphragm.

func setExposureModeCustom(duration: CMTime, iso: Float, completionHandler: ((CMTime) -> Void)?)

Sets the exposure mode to a custom state, and locks exposure duration and ISO at explicit values.

