

- AVFoundation
- AVCaptureDevice
-  isWhiteBalanceModeSupported(\_:) 

Instance Method

# isWhiteBalanceModeSupported(\_:)

Returns a Boolean value that indicates whether the device supports the specified white balance mode.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
func isWhiteBalanceModeSupported(_ whiteBalanceMode: AVCaptureDevice.WhiteBalanceMode) -> Bool
```

## Parameters 

`whiteBalanceMode`  

A white balance mode to use.

## Return Value

true if the device supports the white balance mode; otherwise, false.

## See Also

### Configuring Automatic White Balance

var whiteBalanceMode: AVCaptureDevice.WhiteBalanceMode

The current white balance mode.

enum WhiteBalanceMode

Constants to specify the white balance mode of a capture device.

