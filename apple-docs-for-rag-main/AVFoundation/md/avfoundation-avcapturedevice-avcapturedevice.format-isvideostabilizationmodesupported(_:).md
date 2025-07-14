

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.Format
-  isVideoStabilizationModeSupported(\_:) 

Instance Method

# isVideoStabilizationModeSupported(\_:)

A Boolean value that indicates whether the format supports a given video stabilization mode.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
func isVideoStabilizationModeSupported(_ videoStabilizationMode: AVCaptureVideoStabilizationMode) -> Bool
```

## Parameters 

`videoStabilizationMode`  

The stabilization mode to test.

## Return Value

true if video stabilization is supported; otherwise, false.

## See Also

### Determining Video Stabilization Support

enum AVCaptureVideoStabilizationMode

An enumeration of video stabilization modes that capture devices and formats support.

