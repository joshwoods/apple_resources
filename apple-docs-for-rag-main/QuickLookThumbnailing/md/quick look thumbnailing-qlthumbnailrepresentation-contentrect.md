

- Quick Look Thumbnailing
- QLThumbnailRepresentation
-  contentRect 

Instance Property

# contentRect

The rectangle within the thumbnail image of the document that represents its contents.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
var contentRect: CGRect { get }
```

## Discussion

In icon mode, the content rectangle is the undecorated rectangle, or frame, that the image sits in.

## See Also

### Thumbnail Images

var cgImage: CGImage

A thumbnail in the form of a Core Graphics image object.

var nsImage: NSImage

A thumbnail in the form of an AppKit image object.

var uiImage: UIImage

A thumbnail in the form of a UIKit image object.

var type: QLThumbnailRepresentation.RepresentationType

The type of thumbnail.

enum RepresentationType

The different types of thumbnails that you can create.

