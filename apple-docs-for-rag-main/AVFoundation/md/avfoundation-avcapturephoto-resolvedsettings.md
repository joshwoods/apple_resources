

- AVFoundation
- AVCapturePhoto
-  resolvedSettings 

Instance Property

# resolvedSettings

The settings object that was used to request this photo capture.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+

``` source
var resolvedSettings: AVCaptureResolvedPhotoSettings { get }
```

## Discussion

To determine which capturePhoto(with:delegate:) call produced this photo capture result, match this AVCaptureResolvedPhotoSettings object’s uniqueID value to the uniqueID property of the photo settings object you requested capture with. You can also use this object to find out which values the photo output has chosen for automatic settings.

## See Also

### Resolving Photo Capture Requests

var photoCount: Int

The 1-based index of this photo capture relative to other results from the same capture request.

var timestamp: CMTime

The time at which the image was captured.

