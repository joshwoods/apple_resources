

- AVFoundation
- AVCaptureDevice
-  lensAperture 

Instance Property

# lensAperture

The size of the lens diaphragm.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var lensAperture: Float { get }
```

## Discussion

The value of this property is a float indicating the size (the `f` number) of the lens diaphragm.

This value doesn’t change.

## See Also

### Configuring Exposure Manually

var exposureDuration: CMTime

The length of time over which exposure takes place.

var activeMaxExposureDuration: CMTime

The maximum exposure duration, in seconds, defined in the autoexposure algorithm.

var iso: Float

The current exposure ISO value.

func setExposureModeCustom(duration: CMTime, iso: Float, completionHandler: ((CMTime) -> Void)?)

Sets the exposure mode to a custom state, and locks exposure duration and ISO at explicit values.

