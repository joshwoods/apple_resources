

- AVFoundation
- AVCapturePhotoCaptureDelegate
-  photoOutput(\_:didFinishProcessingLivePhotoToMovieFileAt:duration:photoDisplayTime:resolvedSettings:error:) 

Instance Method

# photoOutput(\_:didFinishProcessingLivePhotoToMovieFileAt:duration:photoDisplayTime:resolvedSettings:error:)

Provides the delegate the movie file URL resulting from a Live Photo capture.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
optional func photoOutput(
    _ output: AVCapturePhotoOutput,
    didFinishProcessingLivePhotoToMovieFileAt outputFileURL: URL,
    duration: CMTime,
    photoDisplayTime: CMTime,
    resolvedSettings: AVCaptureResolvedPhotoSettings,
    error: (any Error)?
)
```

## Parameters 

`output`  

The photo output performing the capture.

`outputFileURL`  

The file URL at which the movie content of the Live Photo was written.

`duration`  

The duration of the Live Photo movie.

`photoDisplayTime`  

The timestamp within the movie to which the still image part of the Live Photo corresponds.

`resolvedSettings`  

An object describing the settings used for this capture. Match this object’s uniqueID value to the uniqueID property of the photo settings object you initiated capture with to determine which capture request this delegate call corresponds to. You can also use this object to find out which values the photo output has chosen for automatic settings.

`error`  

If the capture process could not proceed successfully, an error object describing the failure; otherwise, `nil`.

## Mentioned in 

Tracking Photo Capture Progress

Capturing and Saving Live Photos

## Discussion

Use this method to receive the results of a Live Photo capture. When the photo output calls this method, the movie component of the Live Photo has been written to the location specified by the `outputFileURL` parameter and the Live Photo is ready for consumption. (To receive the still image component of the Live Photo, implement the photoOutput(_:didFinishProcessingPhoto:previewPhoto:resolvedSettings:bracketSettings:error:) method.)

Tip

To add captured Live Photos to the user’s Photos library, use the PHAssetCreationRequest class. To use Live Photos from the Photos library, use the PHLivePhoto and PHLivePhotoView classes. To display Live Photo content on the web, use the LivePhotosKit JS framework.

You don’t need to implement this method if you’re not requesting Live Photo capture.

Important

You must implement this method if you request Live Photo capture (by setting the livePhotoMovieFileURL property of your photo settings object). The photo output validates this requirement when you call its capturePhoto(with:delegate:) method; if your delegate does not implement the correct methods, the photo output raises an exception.

The photo output calls this method only once for each Live Photo capture.

## See Also

### Receiving Capture Results

func photoOutput(AVCapturePhotoOutput, didFinishProcessingPhoto: AVCapturePhoto, error: (any Error)?)

Provides the delegate with the captured image and associated metadata resulting from a photo capture.

func photoOutput(AVCapturePhotoOutput, didFinishRecordingLivePhotoMovieForEventualFileAt: URL, resolvedSettings: AVCaptureResolvedPhotoSettings)

Notifies the delegate that the movie content of a Live Photo has finished recording.

func photoOutput(AVCapturePhotoOutput, didFinishCapturingDeferredPhotoProxy: AVCaptureDeferredPhotoProxy?, error: (any Error)?)

Tells the delegate when the system finishes capturing the photo proxy.

func photoOutput(AVCapturePhotoOutput, didFinishProcessingPhoto: CMSampleBuffer?, previewPhoto: CMSampleBuffer?, resolvedSettings: AVCaptureResolvedPhotoSettings, bracketSettings: AVCaptureBracketedStillImageSettings?, error: (any Error)?)

Provides the delegate a captured image in a processed format (such as JPEG).

Deprecated

func photoOutput(AVCapturePhotoOutput, didFinishProcessingRawPhoto: CMSampleBuffer?, previewPhoto: CMSampleBuffer?, resolvedSettings: AVCaptureResolvedPhotoSettings, bracketSettings: AVCaptureBracketedStillImageSettings?, error: (any Error)?)

Provides the delegate a captured image in RAW format.

Deprecated

