

- AVFoundation
- AVCaptureStillImageOutput
-  captureStillImageAsynchronously(from:completionHandler:) Deprecated

Instance Method

# captureStillImageAsynchronously(from:completionHandler:)

Initiates a still image capture and returns immediately.

iOS 4.0–10.0DeprecatediPadOS 4.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.7–10.15Deprecated

``` source
func captureStillImageAsynchronously(
    from connection: AVCaptureConnection,
    completionHandler handler: @escaping (CMSampleBuffer?, (any Error)?) -> Void
)
```

Deprecated

Use AVCapturePhotoOutput instead.

## Parameters 

`connection`  

The connection from which to capture the image.

`handler`  

A block to invoke after the image has been captured. The block parameters are as follows:

imageDataSampleBuffer  
The data that was captured.

The buffer attachments may contain metadata appropriate to the image data format. For example, a buffer containing JPEG data may carry a kCGImagePropertyExifDictionary as an attachment. See ImageIO/CGImageProperties.h for a list of keys and value types.

error  
If the request could not be completed, an `NSError` object that describes the problem; otherwise `nil`.

## Discussion

This method returns immediately after it is invoked, later calling the provided completion handler block when image data is ready. If the request could not be completed, the error parameter will contain an `NSError` object describing the failure.

You should not assume that the completion handler will be called on a specific thread.

## See Also

### Capturing an Image

var isCapturingStillImage: Bool

Indicates whether a still image is being captured.

Deprecated

