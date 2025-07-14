

- AVFoundation
- AVCapturePhotoCaptureDelegate
-  photoOutput(\_:didFinishProcessingPhoto:error:) 

Instance Method

# photoOutput(\_:didFinishProcessingPhoto:error:)

Provides the delegate with the captured image and associated metadata resulting from a photo capture.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+

``` source
optional func photoOutput(
    _ output: AVCapturePhotoOutput,
    didFinishProcessingPhoto photo: AVCapturePhoto,
    error: (any Error)?
)
```

## Parameters 

`output`  

The photo output performing the capture.

`photo`  

An object containing the captured image pixel buffer, along with any metadata and attachments captured along with the photo (such as a preview image or depth map).

This parameter is always non-`nil`: if an error prevented successful capture, this object still contains metadata for the intended capture.

`error`  

If the capture process could not proceed successfully, an error object describing the failure; otherwise, `nil`.

## Mentioned in 

Capturing Photos in RAW and Apple ProRAW Formats

Tracking Photo Capture Progress

Capturing Uncompressed Image Data

Capturing a Bracketed Photo Sequence

Capturing Thumbnail and Preview Images

## Discussion

Use this method to receive the results of photo capture regardless of format.

Important

Implementing this method is recommended for all still image (as opposed to Live Photo) capture workflows, and required if you request depth data delivery. The photo output validates this requirement when you call its capturePhoto(with:delegate:) method; if your delegate does not implement the correct methods, the photo output raises an exception.

The photo output calls this method once for each primary image to be delivered in a capture request. If you request capture in both RAW and processed formats, this method fires once for each format. If you request a bracketed capture with multiple exposures, this method fires once for each exposure.

## See Also

### Receiving Capture Results

func photoOutput(AVCapturePhotoOutput, didFinishRecordingLivePhotoMovieForEventualFileAt: URL, resolvedSettings: AVCaptureResolvedPhotoSettings)

Notifies the delegate that the movie content of a Live Photo has finished recording.

func photoOutput(AVCapturePhotoOutput, didFinishProcessingLivePhotoToMovieFileAt: URL, duration: CMTime, photoDisplayTime: CMTime, resolvedSettings: AVCaptureResolvedPhotoSettings, error: (any Error)?)

Provides the delegate the movie file URL resulting from a Live Photo capture.

func photoOutput(AVCapturePhotoOutput, didFinishCapturingDeferredPhotoProxy: AVCaptureDeferredPhotoProxy?, error: (any Error)?)

Tells the delegate when the system finishes capturing the photo proxy.

func photoOutput(AVCapturePhotoOutput, didFinishProcessingPhoto: CMSampleBuffer?, previewPhoto: CMSampleBuffer?, resolvedSettings: AVCaptureResolvedPhotoSettings, bracketSettings: AVCaptureBracketedStillImageSettings?, error: (any Error)?)

Provides the delegate a captured image in a processed format (such as JPEG).

Deprecated

func photoOutput(AVCapturePhotoOutput, didFinishProcessingRawPhoto: CMSampleBuffer?, previewPhoto: CMSampleBuffer?, resolvedSettings: AVCaptureResolvedPhotoSettings, bracketSettings: AVCaptureBracketedStillImageSettings?, error: (any Error)?)

Provides the delegate a captured image in RAW format.

Deprecated

