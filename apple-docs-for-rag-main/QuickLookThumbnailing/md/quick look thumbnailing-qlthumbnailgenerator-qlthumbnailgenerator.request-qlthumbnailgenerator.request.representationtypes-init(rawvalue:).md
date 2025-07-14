

- Quick Look Thumbnailing
- QLThumbnailGenerator
- QLThumbnailGenerator.Request
- QLThumbnailGenerator.Request.RepresentationTypes
-  init(rawValue:) 

Initializer

# init(rawValue:)

Creates a new thumbnail type object for a given value.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
init(rawValue: UInt)
```

## See Also

### Creating a Thumbnail Type

static var all: QLThumbnailGenerator.Request.RepresentationTypes

The thumbnail type to generate all possible thumbnail representations.

static var icon: QLThumbnailGenerator.Request.RepresentationTypes

A file icon representation of a file.

static var lowQualityThumbnail: QLThumbnailGenerator.Request.RepresentationTypes

A faster to generate version of the thumbnail that may sacrifice quality for speed.

static var thumbnail: QLThumbnailGenerator.Request.RepresentationTypes

A thumbnail representation of a file.

