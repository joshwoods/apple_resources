

- Quick Look Thumbnailing
- QLThumbnailGenerator
- QLThumbnailGenerator.Request
-  scale 

Instance Property

# scale

The pixel density of the display on the intended device.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
var scale: CGFloat { get }
```

## Discussion

This property represents the scale factor, or pixel density, of the device’s display as described in Image Size and Resolution. For example, the value for a device with a `@2x` display is `2.0`.

You can pass the initializer a screen scale that isn’t the current device’s screen scale. For example, you can create thumbnails for different scales, upload them to a server, and download them later on devices with a different screen scale.

## See Also

### Describing the Requested Thumbnail

var size: CGSize

The size of the thumbnails.

var contentType: UTType!

The content type of the source data for the thumbnail request.

var representationTypes: QLThumbnailGenerator.Request.RepresentationTypes

The thumbnail sizes that you provide for a thumbnail request.

var minimumDimension: CGFloat

The minimum height or width for a generated thumbnail.

var iconMode: Bool

A Boolean value indicating whether the generated thumbnail request should include icon decorations.

struct RepresentationTypes

The various types of thumbnails that you can request.

