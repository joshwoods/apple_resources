

- AVFoundation
- AVCapturePhotoCaptureDelegate
-  photoOutput(\_:didFinishCapturingDeferredPhotoProxy:error:) 

Instance Method

# photoOutput(\_:didFinishCapturingDeferredPhotoProxy:error:)

Tells the delegate when the system finishes capturing the photo proxy.

iOS 17.0+iPadOS 17.0+

``` source
optional func photoOutput(
    _ output: AVCapturePhotoOutput,
    didFinishCapturingDeferredPhotoProxy deferredPhotoProxy: AVCaptureDeferredPhotoProxy?,
    error: (any Error)?
)
```

## Parameters 

`output`  

The output instance.

`deferredPhotoProxy`  

A AVCaptureDeferredPhotoProxy instance that contains a proxy CVPixelBuffer as a placeholder for the final image.

`error`  

If the system couldn’t create the photo proxy, or any of the underlying intermediate files, an error object that describes the failure.

## Discussion

You can use the output’s fileDataRepresentation() with PHAssetCreationRequest to eventually produce the final, processed photo into the user’s Photo Library. Add the in-memory proxy file data representation to the photo library as quickly as possible after this call to ensure that the photo library can begin background processing. It’s also important so that the intermediates aren’t removed by a periodic clean-up job looking for abandoned intermediates produced by using the deferred photo processing APIs.

Your delegate implementation must adopt this method to opt into deferred photo processing, otherwise calling capturePhoto(with:delegate:) throws an exception.

## See Also

### Receiving Capture Results

func photoOutput(AVCapturePhotoOutput, didFinishProcessingPhoto: AVCapturePhoto, error: (any Error)?)

Provides the delegate with the captured image and associated metadata resulting from a photo capture.

func photoOutput(AVCapturePhotoOutput, didFinishRecordingLivePhotoMovieForEventualFileAt: URL, resolvedSettings: AVCaptureResolvedPhotoSettings)

Notifies the delegate that the movie content of a Live Photo has finished recording.

func photoOutput(AVCapturePhotoOutput, didFinishProcessingLivePhotoToMovieFileAt: URL, duration: CMTime, photoDisplayTime: CMTime, resolvedSettings: AVCaptureResolvedPhotoSettings, error: (any Error)?)

Provides the delegate the movie file URL resulting from a Live Photo capture.

func photoOutput(AVCapturePhotoOutput, didFinishProcessingPhoto: CMSampleBuffer?, previewPhoto: CMSampleBuffer?, resolvedSettings: AVCaptureResolvedPhotoSettings, bracketSettings: AVCaptureBracketedStillImageSettings?, error: (any Error)?)

Provides the delegate a captured image in a processed format (such as JPEG).

Deprecated

func photoOutput(AVCapturePhotoOutput, didFinishProcessingRawPhoto: CMSampleBuffer?, previewPhoto: CMSampleBuffer?, resolvedSettings: AVCaptureResolvedPhotoSettings, bracketSettings: AVCaptureBracketedStillImageSettings?, error: (any Error)?)

Provides the delegate a captured image in RAW format.

Deprecated

