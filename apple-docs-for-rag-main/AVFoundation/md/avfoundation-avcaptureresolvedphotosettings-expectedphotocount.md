

- AVFoundation
- AVCaptureResolvedPhotoSettings
-  expectedPhotoCount 

Instance Property

# expectedPhotoCount

The number of photo capture results in the capture request.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+

``` source
var expectedPhotoCount: Int { get }
```

## Mentioned in 

Capturing a Bracketed Photo Sequence

Tracking Photo Capture Progress

## Discussion

When you request a photo capture, the photo output calls your delegate’s photoOutput(_:didFinishProcessingPhoto:error:) method many times based on the settings you choose. For example, if you request a bracket of three exposures with image delivery in both JPEG and RAW formats, the expected photo count is `6`.

The photoCount property of each AVCapturePhoto object delivered to your delegate indicates where that capture result relates to this sequence. When your delegate receives a photo whose photoCount value matches the expectedPhotoCount, you know you’ve received the last one for the given capture request.

## See Also

### Resolving Photo Capture Requests

var uniqueID: Int64

The unique identifier for the photo capture this settings object corresponds to.

