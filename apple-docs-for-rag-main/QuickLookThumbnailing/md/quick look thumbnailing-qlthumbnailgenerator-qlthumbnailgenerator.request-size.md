

- Quick Look Thumbnailing
- QLThumbnailGenerator
- QLThumbnailGenerator.Request
-  size 

Instance Property

# size

The size of the thumbnails.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
var size: CGSize { get }
```

## See Also

### Describing the Requested Thumbnail

var scale: CGFloat

The pixel density of the display on the intended device.

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

