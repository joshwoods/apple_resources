

- Quick Look Thumbnailing
- QLFileThumbnailRequest
-  maximumSize 

Instance Property

# maximumSize

The maximum accepted size of a thumbnail.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
var maximumSize: CGSize { get }
```

## Discussion

The `maximumSize` accepted is also the preferred size of the thumbnail that you need to create. Your generated thumbnail’s width or height should match the `width` or `height` of the `maximumSize`, or, ideally, both.

## See Also

### Describing the Requested Thumbnail

var minimumSize: CGSize

The minimum accepted size of a thumbnail.

var scale: CGFloat

The scale of the requested thumbnail.

var fileURL: URL

The URL of the image file to use for the thumbnail.

