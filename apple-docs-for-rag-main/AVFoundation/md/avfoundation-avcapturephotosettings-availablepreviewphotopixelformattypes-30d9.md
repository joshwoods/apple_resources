

- AVFoundation
- AVCapturePhotoSettings
-  availablePreviewPhotoPixelFormatTypes 

Instance Property

# availablePreviewPhotoPixelFormatTypes

An array of available of pixel format types available to specify a preview photo format.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+macOS 11.0+tvOS 17.0+

``` source
@nonobjc
var availablePreviewPhotoPixelFormatTypes: [OSType] { get }
```

## Discussion

The array is sorted so that preview formats requiring fewer conversions come first.

## See Also

### Enabling Preview and Thumbnail Delivery

var previewPhotoFormat: [String : Any]?

A dictionary describing the format for delivery of preview-sized images alongside the main photo.

var embeddedThumbnailPhotoFormat: [String : Any]?

A dictionary describing the format for delivery of thumbnail images embedded in photo file output.

var availableRawEmbeddedThumbnailPhotoCodecTypes: [AVVideoCodecType]

An array of video codec types compatible with the photo settings for embedding raw thumbnail images in photo file output.

var rawEmbeddedThumbnailPhotoFormat: [String : Any]?

A dictionary describing the format for delivery of raw thumbnail images embedded in photo file output.

var availableEmbeddedThumbnailPhotoCodecTypes: [AVVideoCodecType]

An array of video codec types compatible with the photo settings for embedding thumbnail images in photo file output.

