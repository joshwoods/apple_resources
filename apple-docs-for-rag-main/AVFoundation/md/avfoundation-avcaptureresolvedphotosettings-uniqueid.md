

- AVFoundation
- AVCaptureResolvedPhotoSettings
-  uniqueID 

Instance Property

# uniqueID

The unique identifier for the photo capture this settings object corresponds to.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+

``` source
var uniqueID: Int64 { get }
```

## Mentioned in 

Tracking Photo Capture Progress

## Discussion

The value of this property matches the matches the uniqueID value of the AVCapturePhotoSettings object you passed when initiating a photo capture with the capturePhoto(with:delegate:) method. Use this value to determine which delegate method calls correspond to which capture requests.

## See Also

### Resolving Photo Capture Requests

var expectedPhotoCount: Int

The number of photo capture results in the capture request.

