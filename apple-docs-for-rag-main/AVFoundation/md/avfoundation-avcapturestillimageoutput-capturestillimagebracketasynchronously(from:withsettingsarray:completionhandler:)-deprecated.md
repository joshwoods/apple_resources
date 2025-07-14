

- AVFoundation
- AVCaptureStillImageOutput
-  captureStillImageBracketAsynchronously(from:withSettingsArray:completionHandler:) Deprecated

Instance Method

# captureStillImageBracketAsynchronously(from:withSettingsArray:completionHandler:)

Captures a still image bracket.

iOS 8.0–10.0DeprecatediPadOS 8.0–10.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
func captureStillImageBracketAsynchronously(
    from connection: AVCaptureConnection,
    withSettingsArray settings: [AVCaptureBracketedStillImageSettings],
    completionHandler handler: @escaping (CMSampleBuffer?, AVCaptureBracketedStillImageSettings?, (any Error)?) -> Void
)
```

Deprecated

Use AVCapturePhotoOutput capturePhotoWithSettings:delegate: instead.

## Parameters 

`connection`  

The connection through which the still image bracket should be captured.

`settings`  

An array of AVCaptureBracketedStillImageSettings objects. All the array items must be of the same AVCaptureBracketedStillImageSettings subclass, or an invalidArgumentException exception is thrown.

`handler`  

A user provided block that will be called asynchronously as each still image in the bracket is captured.

The block has three parameters:

sampleBuffer  
If the capture request is successful, contains a valid CMSampleBuffer.

stillImageSettings  
Contains the AVCaptureBracketedStillImageSettings object corresponding to this still image.

error  
If the bracketed capture fails, `sampleBuffer` is `NULL` and error is non-`nil`.

If the count of the `settings` parameter exceeds maxBracketedCaptureStillImageCount, then `AVErrorMaximumStillImageCaptureRequestsExceeded` is returned.

You should not assume that the completion handler will be called on a specific thread.

## Discussion

If you have not invoked prepareToCaptureStillImageBracket(from:withSettingsArray:completionHandler:) for this still image bracket request, the bracket may not be taken immediately, as the receiver may internally need to prepare resources.

## See Also

### Related Documentation

func captureStillImageAsynchronously(from: AVCaptureConnection, completionHandler: (CMSampleBuffer?, (any Error)?) -> Void)

Initiates a still image capture and returns immediately.

Deprecated

### Still Image Bracketed Capture

var maxBracketedCaptureStillImageCount: Int

Specifies the maximum number of still images that may be taken in a single bracket.

Deprecated

func prepareToCaptureStillImageBracket(from: AVCaptureConnection, withSettingsArray: [AVCaptureBracketedStillImageSettings], completionHandler: (Bool, (any Error)?) -> Void)

Allows the receiver to prepare resources in advance of capturing a still image bracket.

Deprecated

var isLensStabilizationDuringBracketedCaptureSupported: Bool

A Boolean value that indicates whether the capture output supports lens stabilization across the duration of a bracketed capture.

Deprecated

var isLensStabilizationDuringBracketedCaptureEnabled: Bool

A Boolean value that specifies whether to stabilize the lens across the duration of a bracketed capture.

Deprecated

