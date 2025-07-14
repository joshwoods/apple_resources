

- AVFoundation
- AVCaptureDevice
-  setExposureModeCustom(duration:iso:completionHandler:) 

Instance Method

# setExposureModeCustom(duration:iso:completionHandler:)

Sets the exposure mode to a custom state, and locks exposure duration and ISO at explicit values.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
func setExposureModeCustom(
    duration: CMTime,
    iso ISO: Float,
    completionHandler handler: ((CMTime) -> Void)? = nil
)
```

``` source
func setExposureModeCustom(
    duration: CMTime,
    iso ISO: Float
) async -> CMTime
```

## Parameters 

`duration`  

The exposure duration.

Pass a value of currentExposureDuration to leave the current exposure duration unchanged.

Changes made to the exposure duration may result in changes to activeVideoMinFrameDuration or activeVideoMaxFrameDuration.

`ISO`  

The exposure ISO value.

Pass a value of currentISO to leave the current ISO unchanged.

`handler`  

A callback the system invokes when the adjustment to the exposure duration and ISO is complete. If you call this method multiple times, the system calls the completion handlers in FIFO order.

The system passes a time value that matches that of the first buffer to which its applied all settings. It synchronizes the timestamp to the device clock, and you must convert the timestamp to the synchronizationClock prior to comparison with the timestamps of buffers delivered through an AVCaptureVideoDataOutput.

You can pass `nil` for this parameter if you don’t require this information.

## Discussion

This method throws an exception if you set the exposure duration or ISO values to an unsupported level

Before changing exposure mode, you must call lockForConfiguration() to acquire exclusive access to the device’s configuration properties. Otherwise, setting the value of this property raises an exception. When you finish configuring the device, call unlockForConfiguration() to release the lock and allow other devices to configure the settings.

When using AVCapturePhotoOutput to capture photos, the photoQualityPrioritization property of AVCapturePhotoSettings defaults to AVCapturePhotoOutput.QualityPrioritization.balanced, which allows photo capture to temporarily override the capture device’s exposure duration and ISO if the scene is dark enough to require multi-image fusion to improve quality. To ensure that the system honors the device exposure duration and ISO values while in AVCaptureDevice.ExposureMode.custom or AVCaptureDevice.ExposureMode.locked mode, you must photo quality prioritization to AVCapturePhotoOutput.QualityPrioritization.speed.

## Topics

### Exposure Constants

class let currentExposureDuration: CMTime

A special constant representing the current exposure duration setting.

class let currentISO: Float

A constant to indicate not to specify a new ISO value, and instead set it to its current value.

## See Also

### Configuring Exposure Manually

var exposureDuration: CMTime

The length of time over which exposure takes place.

var activeMaxExposureDuration: CMTime

The maximum exposure duration, in seconds, defined in the autoexposure algorithm.

var iso: Float

The current exposure ISO value.

var lensAperture: Float

The size of the lens diaphragm.

