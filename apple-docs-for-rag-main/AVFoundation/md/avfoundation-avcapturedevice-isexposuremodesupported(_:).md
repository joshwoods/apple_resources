

- AVFoundation
- AVCaptureDevice
-  isExposureModeSupported(\_:) 

Instance Method

# isExposureModeSupported(\_:)

Returns a Boolean value that indicates whether a device supports the specified exposure mode.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
func isExposureModeSupported(_ exposureMode: AVCaptureDevice.ExposureMode) -> Bool
```

## Parameters 

`exposureMode`  

An exposure mode to query.

## Return Value

true if `exposureMode` is supported; otherwise, false.

## See Also

### Managing the Exposure Mode

var exposureMode: AVCaptureDevice.ExposureMode

The exposure mode for the device.

enum ExposureMode

Constants that specify the exposure mode of a capture device.

