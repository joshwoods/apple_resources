

- Quick Look Thumbnailing
- QLThumbnailGenerator
- QLThumbnailGenerator.Request
-  minimumDimension 

Instance Property

# minimumDimension

The minimum height or width for a generated thumbnail.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
var minimumDimension: CGFloat { get set }
```

## Discussion

This property defines a minimum dimension for a generated thumbnail, returning a thumbnail with a width or height greater or equal to the value of `minimumDimension` \* scale.

The default value for this property is `0`.

If you set this property, and the system can’t generate a thumbnail of `minimumDimension` for any of the requested types represented by QLThumbnailGenerator.Request.RepresentationTypes, then QLThumbnailGenerator doesn’t generate a thumbnail.

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

var iconMode: Bool

A Boolean value indicating whether the generated thumbnail request should include icon decorations.

struct RepresentationTypes

The various types of thumbnails that you can request.

