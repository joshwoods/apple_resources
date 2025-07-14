

- AVFoundation
- AVCaptureDevice
-  setExposureTargetBias(\_:completionHandler:) 

Instance Method

# setExposureTargetBias(\_:completionHandler:)

Sets the bias to apply to the target exposure value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
func setExposureTargetBias(
    _ bias: Float,
    completionHandler handler: ((CMTime) -> Void)? = nil
)
```

``` source
func setExposureTargetBias(_ bias: Float) async -> CMTime
```

## Parameters 

`bias`  

The bias to apply to the exposure target value.

`handler`  

A callback the system invokes when the adjustment to the exposure target bias is complete. If you call this method multiple times, the system calls the completion handlers in FIFO order.

The system passes a time value that matches that of the first buffer to which its applied all settings. It synchronizes the timestamp to the device clock, and you must convert the timestamp to the synchronizationClock prior to comparison with the timestamps of buffers delivered through an AVCaptureVideoDataOutput.

You can pass `nil` for this parameter if you don’t require this information.

## Discussion

Before changing the value the lens position, you must call lockForConfiguration() to acquire exclusive access to the device’s configuration properties. Otherwise, setting the value of this property raises an exception. When you finish configuring the device, call unlockForConfiguration() to release the lock and allow other devices to configure the settings.

## See Also

### Adjusting Exposure Compensation

var exposureTargetOffset: Float

The metered exposure level’s offset from the target exposure value, in exposure value (EV) units.

var exposureTargetBias: Float

The bias to apply to the target exposure value, in exposure value (EV) units.

var minExposureTargetBias: Float

The minimum supported exposure bias, in exposure value (EV) units.

var maxExposureTargetBias: Float

The maximum supported exposure bias, in exposure value (EV) units.

class let currentExposureTargetBias: Float

A special constant that represents the current exposure bias value.

