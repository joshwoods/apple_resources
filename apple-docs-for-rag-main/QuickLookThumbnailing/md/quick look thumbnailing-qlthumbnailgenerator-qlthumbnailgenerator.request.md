

- Quick Look Thumbnailing
- QLThumbnailGenerator
-  QLThumbnailGenerator.Request 

Class

# QLThumbnailGenerator.Request

A request to generate a thumbnail for a file.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
class Request
```

## Topics

### Creating a Thumbail Request

init(fileAt: URL, size: CGSize, scale: CGFloat, representationTypes: QLThumbnailGenerator.Request.RepresentationTypes)

Creates a new request for a thumbnail with the specified parameters for a file at a provided URL.

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

var iconMode: Bool

A Boolean value indicating whether the generated thumbnail request should include icon decorations.

struct RepresentationTypes

The various types of thumbnails that you can request.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Generating a Thumbnail

func generateBestRepresentation(for: QLThumbnailGenerator.Request, completion: (QLThumbnailRepresentation?, (any Error)?) -> Void)

Generates the best possible thumbnail representation for a file and calls a handler upon completion.

func generateRepresentations(for: QLThumbnailGenerator.Request, update: ((QLThumbnailRepresentation?, QLThumbnailRepresentation.RepresentationType, (any Error)?) -> Void)?)

Generates various thumbnail representations for a file and calls the update handler for each thumbnail representation.

