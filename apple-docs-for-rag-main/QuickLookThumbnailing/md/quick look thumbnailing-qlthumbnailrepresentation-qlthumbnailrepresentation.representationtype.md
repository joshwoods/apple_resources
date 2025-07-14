

- Quick Look Thumbnailing
- QLThumbnailRepresentation
-  QLThumbnailRepresentation.RepresentationType 

Enumeration

# QLThumbnailRepresentation.RepresentationType

The different types of thumbnails that you can create.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
enum RepresentationType
```

## Mentioned in 

Providing Thumbnails of Your Custom File Types

## Topics

### Enumeration Cases

case icon

A file icon representation of an image.

case lowQualityThumbnail

A cached thumbnail representation of an image.

case thumbnail

A thumbnail representation of an image.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

var contentRect: CGRect

The rectangle within the thumbnail image of the document that represents its contents.

