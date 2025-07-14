

- AVFoundation
- AVCapturePhotoSettings
-  availableEmbeddedThumbnailPhotoCodecTypes 

Instance Property

# availableEmbeddedThumbnailPhotoCodecTypes

An array of video codec types compatible with the photo settings for embedding thumbnail images in photo file output.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var availableEmbeddedThumbnailPhotoCodecTypes: [AVVideoCodecType] { get }
```

## Discussion

To enable embedding thumbnail images in photo file output, set the embeddedThumbnailPhotoFormat property using one of the codec types listed in this array.

The order of this array is such that the most backward-compatible codec is listed first.

## See Also

### Enabling Preview and Thumbnail Delivery

var previewPhotoFormat: [String : Any]?

A dictionary describing the format for delivery of preview-sized images alongside the main photo.

var availablePreviewPhotoPixelFormatTypes: [OSType]

An array of available of pixel format types available to specify a preview photo format.

var embeddedThumbnailPhotoFormat: [String : Any]?

A dictionary describing the format for delivery of thumbnail images embedded in photo file output.

var availableRawEmbeddedThumbnailPhotoCodecTypes: [AVVideoCodecType]

An array of video codec types compatible with the photo settings for embedding raw thumbnail images in photo file output.

var rawEmbeddedThumbnailPhotoFormat: [String : Any]?

A dictionary describing the format for delivery of raw thumbnail images embedded in photo file output.

