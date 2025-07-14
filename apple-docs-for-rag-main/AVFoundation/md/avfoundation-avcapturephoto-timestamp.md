

- AVFoundation
- AVCapturePhoto
-  timestamp 

Instance Property

# timestamp

The time at which the image was captured.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+

``` source
var timestamp: CMTime { get }
```

## Discussion

This timestamp is always synchronized to the masterClock time of the AVCaptureSession object to which the photo output is connected.

## See Also

### Resolving Photo Capture Requests

var resolvedSettings: AVCaptureResolvedPhotoSettings

The settings object that was used to request this photo capture.

var photoCount: Int

The 1-based index of this photo capture relative to other results from the same capture request.

