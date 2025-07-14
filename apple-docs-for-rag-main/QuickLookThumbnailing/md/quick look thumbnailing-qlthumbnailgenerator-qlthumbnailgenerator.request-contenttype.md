

- Quick Look Thumbnailing
- QLThumbnailGenerator
- QLThumbnailGenerator.Request
-  contentType 

Instance Property

# contentType

The content type of the source data for the thumbnail request.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
var contentType: UTType! { get set }
```

## Discussion

Quick Look Thumbnailing uses the content type of the source data to determine the provider of the thumbnail and the icon styles it applies when you request iconMode.

If you don’t set this property, Quick Look Thumbnailing derives the content from the file extension. When the file doesn’t have a meaningful extension and you know the content type, set the property directly.

## See Also

### Describing the Requested Thumbnail

var size: CGSize

The size of the thumbnails.

var scale: CGFloat

The pixel density of the display on the intended device.

var representationTypes: QLThumbnailGenerator.Request.RepresentationTypes

The thumbnail sizes that you provide for a thumbnail request.

var minimumDimension: CGFloat

The minimum height or width for a generated thumbnail.

var iconMode: Bool

A Boolean value indicating whether the generated thumbnail request should include icon decorations.

struct RepresentationTypes

The various types of thumbnails that you can request.

