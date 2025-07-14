

- AVFoundation
- AVCaptureStillImageOutput
-  prepareToCaptureStillImageBracket(from:withSettingsArray:completionHandler:) Deprecated

Instance Method

# prepareToCaptureStillImageBracket(from:withSettingsArray:completionHandler:)

Allows the receiver to prepare resources in advance of capturing a still image bracket.

iOS 8.0–10.0DeprecatediPadOS 8.0–10.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
func prepareToCaptureStillImageBracket(
    from connection: AVCaptureConnection,
    withSettingsArray settings: [AVCaptureBracketedStillImageSettings],
    completionHandler handler: @escaping (Bool, (any Error)?) -> Void
)
```

Deprecated

Use AVCapturePhotoOutput setPreparedPhotoSettingsArray:completionHandler: instead.

## Parameters 

`connection`  

The connection through which the still image bracket should be captured.

`settings`  

An array of AVCaptureBracketedStillImageSettings objects. All the array items must be of the same AVCaptureBracketedStillImageSettings subclass, or an invalidArgumentException exception is thrown.

`handler`  

A user provided block that will be called asynchronously once resources have successfully been allocated for the specified bracketed capture operation.

The block has two parameters:

prepared  
If sufficient resources could not be allocated, this parameter is false, and the `error` parameter contains a non-`nil` error value.

error  
The value is non-`nil` if an error is encountered.

If the count of the `settings` parameter exceeds maxBracketedCaptureStillImageCount, then `AVErrorMaximumStillImageCaptureRequestsExceeded` is returned.

You should not assume that the completion handler will be called on a specific thread.

## Discussion

Before taking a still image bracket, additional resources may need to be allocated. By calling this method first, you are able to know when the receiver is ready to capture the bracket with the specified settings array.

## See Also

### Related Documentation

func captureStillImageAsynchronously(from: AVCaptureConnection, completionHandler: (CMSampleBuffer?, (any Error)?) -> Void)

Initiates a still image capture and returns immediately.

Deprecated

### Still Image Bracketed Capture

func captureStillImageBracketAsynchronously(from: AVCaptureConnection, withSettingsArray: [AVCaptureBracketedStillImageSettings], completionHandler: (CMSampleBuffer?, AVCaptureBracketedStillImageSettings?, (any Error)?) -> Void)

Captures a still image bracket.

Deprecated

var maxBracketedCaptureStillImageCount: Int

Specifies the maximum number of still images that may be taken in a single bracket.

Deprecated

var isLensStabilizationDuringBracketedCaptureSupported: Bool

A Boolean value that indicates whether the capture output supports lens stabilization across the duration of a bracketed capture.

Deprecated

var isLensStabilizationDuringBracketedCaptureEnabled: Bool

A Boolean value that specifies whether to stabilize the lens across the duration of a bracketed capture.

Deprecated

