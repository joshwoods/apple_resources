

- Quick Look Thumbnailing
- QLThumbnailGenerator
- QLThumbnailGenerator.Request
-  iconMode 

Instance Property

# iconMode

A Boolean value indicating whether the generated thumbnail request should include icon decorations.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
var iconMode: Bool { get set }
```

## Discussion

Set this property to true to generate a thumbnail that’s appropriate to use as a file icon. Depending on the platform, the thumbnail may be embedded in a frame, show a curled corner, or display a background or drop shadow. If this property’s value is false, QLThumbnailGenerator generates a raw, undecorated thumbnail.

The default value of this property is false.

## See Also

### Describing the Requested Thumbnail

var size: CGSize

The size of the thumbnails.

var scale: CGFloat

The pixel density of the display on the intended device.

var contentType: UTType!

The content type of the source data for the thumbnail request.

var representationTypes: QLThumbnailGenerator.Request.RepresentationTypes

The thumbnail sizes that you provide for a thumbnail request.

var minimumDimension: CGFloat

The minimum height or width for a generated thumbnail.

struct RepresentationTypes

The various types of thumbnails that you can request.

