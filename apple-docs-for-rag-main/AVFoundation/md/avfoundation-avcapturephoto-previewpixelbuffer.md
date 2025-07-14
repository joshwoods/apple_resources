

- AVFoundation
- AVCapturePhoto
-  previewPixelBuffer 

Instance Property

# previewPixelBuffer

The pixel data for a preview-sized version of the photo, if requested.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var previewPixelBuffer: CVPixelBuffer? { get }
```

## Mentioned in 

Capturing Thumbnail and Preview Images

## Discussion

If you requested a preview image by specifying the previewPhotoFormat property of your photo settings when requesting capture, this property offers access to the resulting preview image pixel data. The pixel buffer contains only the minimal attachments required for correct display. If you did not request a preview image, this property’s value is `nil`.

## See Also

### Accessing Preview Photo Data

var embeddedThumbnailPhotoFormat: [String : Any]?

A dictionary describing the data format for a preview-sized image accompanying the captured photo.

