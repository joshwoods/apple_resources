

- AVFoundation
- AVCapturePhoto
-  photoCount 

Instance Property

# photoCount

The 1-based index of this photo capture relative to other results from the same capture request.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+

``` source
var photoCount: Int { get }
```

## Mentioned in 

Tracking Photo Capture Progress

Capturing a Bracketed Photo Sequence

## Discussion

The expectedPhotoCount property of this capture result’s resolvedSettings object indicates the total number of images that will be returned for a given capture request. When your delegate’s photoOutput(_:didFinishProcessingPhoto:error:) method receives a photo whose photoCount value matches the expectedPhotoCount value, you know you’ve received the last one for the given capture request.

## See Also

### Resolving Photo Capture Requests

var resolvedSettings: AVCaptureResolvedPhotoSettings

The settings object that was used to request this photo capture.

var timestamp: CMTime

The time at which the image was captured.

