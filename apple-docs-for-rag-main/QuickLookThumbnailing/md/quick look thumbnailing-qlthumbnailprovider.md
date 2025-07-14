

- Quick Look Thumbnailing
-  QLThumbnailProvider 

Class

# QLThumbnailProvider

An abstract base class for creating thumbnails of custom file types.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
class QLThumbnailProvider
```

## Mentioned in 

Providing Thumbnails of Your Custom File Types

## Topics

### Essentials

func provideThumbnail(for: QLFileThumbnailRequest, (QLThumbnailReply?, (any Error)?) -> Void)

Creates a thumbnail of a custom file type for a specific request.

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

class QLFileThumbnailRequest

A request to generate a thumbnail for a custom file type.

class QLThumbnailReply

The object that provides a thumbnail for a custom file type.

