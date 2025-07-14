

- Quick Look Thumbnailing
-  QLThumbnailReply 

Class

# QLThumbnailReply

The object that provides a thumbnail for a custom file type.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
class QLThumbnailReply
```

## Mentioned in 

Providing Thumbnails of Your Custom File Types

## Topics

### Creating a Thumbnail

convenience init(contextSize: CGSize, currentContextDrawing: () -> Bool)

Creates a new thumbnail for a custom file type in the current context.

convenience init(contextSize: CGSize, drawing: (CGContext) -> Bool)

Creates a new thumbnail for a custom file type in the given context.

convenience init(imageFileURL: URL)

Creates a new thumbnail for a custom file type using a file at the given URL.

### Customizing a Thumbnail Reply

var extensionBadge: String

A short string that identifies the file type that the system uses as a badge when producing an icon thumbnail.

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

class QLFileThumbnailRequest

A request to generate a thumbnail for a custom file type.

