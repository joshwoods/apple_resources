

- Quick Look Thumbnailing
-  QLFileThumbnailRequest 

Class

# QLFileThumbnailRequest

A request to generate a thumbnail for a custom file type.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
class QLFileThumbnailRequest
```

## Topics

### Describing the Requested Thumbnail

var maximumSize: CGSize

The maximum accepted size of a thumbnail.

var minimumSize: CGSize

The minimum accepted size of a thumbnail.

var scale: CGFloat

The scale of the requested thumbnail.

var fileURL: URL

The URL of the image file to use for the thumbnail.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Thumbnails for Custom File Types

Providing Thumbnails of Your Custom File Types

Implement a Thumbnail Extension to allow the operating system and other apps to display thumbnails of your custom files.

class QLThumbnailProvider

An abstract base class for creating thumbnails of custom file types.

class QLThumbnailReply

The object that provides a thumbnail for a custom file type.

