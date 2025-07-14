

- AVFoundation
- AVCaptureDevice
-  activeMaxExposureDuration 

Instance Property

# activeMaxExposureDuration

The maximum exposure duration, in seconds, defined in the autoexposure algorithm.

iOS 12.0+iPadOS 12.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var activeMaxExposureDuration: CMTime { get set }
```

## Discussion

When you set the exposureMode to AVCaptureDevice.ExposureMode.autoExpose or AVCaptureDevice.ExposureMode.continuousAutoExposure, the autoexposure algorithm picks a default maximum exposure duration that’s tuned for the current configuration, balancing low light image quality with motion preservation. By querying or key-value observing this property, you can determine the current maximum exposure duration in use.

You may also override the default value by setting this property to a value between the format’s minExposureDuration and maxExposureDuration values. The system throws an exception if you pass an out-of-bounds exposure value.

Setting the property to the special value of invalid resets the autoexposure maximum duration to the device’s default for your current configuration. When the device’s activeFormat or the capture session’s sessionPreset changes, this property resets to the default max exposure duration for the new format or session preset.

On some devices, the auto exposure algorithm picks a different maximum exposure duration for a given format depending on whether you used the sessionPreset or activeFormat APIs to set to set the format. To ensure uniform default handling of maximum exposure duration, set the value of a capture input’s unifiedAutoExposureDefaultsEnabled property to true.

## See Also

### Configuring Exposure Manually

var exposureDuration: CMTime

The length of time over which exposure takes place.

var iso: Float

The current exposure ISO value.

var lensAperture: Float

The size of the lens diaphragm.

func setExposureModeCustom(duration: CMTime, iso: Float, completionHandler: ((CMTime) -> Void)?)

Sets the exposure mode to a custom state, and locks exposure duration and ISO at explicit values.

