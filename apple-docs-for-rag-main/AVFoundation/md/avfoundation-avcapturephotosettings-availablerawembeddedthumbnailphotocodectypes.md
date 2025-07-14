

- AVFoundation
- AVCapturePhotoSettings
-  availableRawEmbeddedThumbnailPhotoCodecTypes 

Instance Property

# availableRawEmbeddedThumbnailPhotoCodecTypes

An array of video codec types compatible with the photo settings for embedding raw thumbnail images in photo file output.

iOS 12.0+iPadOS 12.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var availableRawEmbeddedThumbnailPhotoCodecTypes: [AVVideoCodecType] { get }
```

## See Also

### Enabling Preview and Thumbnail Delivery

var previewPhotoFormat: [String : Any]?

A dictionary describing the format for delivery of preview-sized images alongside the main photo.

var availablePreviewPhotoPixelFormatTypes: [OSType]

An array of available of pixel format types available to specify a preview photo format.

var embeddedThumbnailPhotoFormat: [String : Any]?

A dictionary describing the format for delivery of thumbnail images embedded in photo file output.

var rawEmbeddedThumbnailPhotoFormat: [String : Any]?

A dictionary describing the format for delivery of raw thumbnail images embedded in photo file output.

var availableEmbeddedThumbnailPhotoCodecTypes: [AVVideoCodecType]

An array of video codec types compatible with the photo settings for embedding thumbnail images in photo file output.

