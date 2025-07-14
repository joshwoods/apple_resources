

- AVFoundation
- AVCapturePhoto
-  embeddedThumbnailPhotoFormat 

Instance Property

# embeddedThumbnailPhotoFormat

A dictionary describing the data format for a preview-sized image accompanying the captured photo.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var embeddedThumbnailPhotoFormat: [String : Any]? { get }
```

## Discussion

See Video settings for possible keys and values.

If you requested an embedded thumbnail image by specifying the embeddedThumbnailPhotoFormat property of your photo settings when requesting capture, this property’s value is the resolved video settings dictionary for the embedded thumbnail image. If you did not request an embedded thumbnail image, this property’s value is `nil`.

## See Also

### Accessing Preview Photo Data

var previewPixelBuffer: CVPixelBuffer?

The pixel data for a preview-sized version of the photo, if requested.

