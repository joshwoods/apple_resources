

- AVFoundation
- AVCapturePhotoSettings
-  previewPhotoFormat 

Instance Property

# previewPhotoFormat

A dictionary describing the format for delivery of preview-sized images alongside the main photo.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var previewPhotoFormat: [String : Any]? { get set }
```

## Mentioned in 

Capturing Thumbnail and Preview Images

## Discussion

By default, this property is `nil`, specifying that the photo output should return only the main image requested. To also receive a preview-sized image, set this property to a dictionary describing the format for that image, containing the following keys and values:

The dictionary must contain the kCVPixelBufferPixelFormatTypeKey key, whose corresponding value must be one of the pixel format types listed in the availablePreviewPhotoPixelFormatTypes array.

Optionally, you can also include the kCVPixelBufferWidthKey and kCVPixelBufferHeightKey keys to specify the size of the preview image. (If you specify either width or height, you must specify both.) If the size you specify does not match the aspect ratio of the primary photo, the photo output provides a preview image whose size matches the longer of the two specified dimensions, preserving the original aspect ratio.

Note

The photo capture system supports both *preview* and *thumbnail* images as companions to the full-size primary image in a photo capture. A preview image is intended for immediate display (as seen when taking photos in the iOS Camera app), and as such is sized for full-screen presentation on the current device. A thumbnail image is intended for embedding in the output image file and can be used by other software (such as Quick Look in a file browser) to allow users to quickly review the image without loading the entire image file; the size of thumbnail images may be limited depending on the output file format.

## See Also

### Enabling Preview and Thumbnail Delivery

var availablePreviewPhotoPixelFormatTypes: [OSType]

An array of available of pixel format types available to specify a preview photo format.

var embeddedThumbnailPhotoFormat: [String : Any]?

A dictionary describing the format for delivery of thumbnail images embedded in photo file output.

var availableRawEmbeddedThumbnailPhotoCodecTypes: [AVVideoCodecType]

An array of video codec types compatible with the photo settings for embedding raw thumbnail images in photo file output.

var rawEmbeddedThumbnailPhotoFormat: [String : Any]?

A dictionary describing the format for delivery of raw thumbnail images embedded in photo file output.

var availableEmbeddedThumbnailPhotoCodecTypes: [AVVideoCodecType]

An array of video codec types compatible with the photo settings for embedding thumbnail images in photo file output.

