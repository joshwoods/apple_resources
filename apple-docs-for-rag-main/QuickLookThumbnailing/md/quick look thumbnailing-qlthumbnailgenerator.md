

- Quick Look Thumbnailing
-  QLThumbnailGenerator 

Class

# QLThumbnailGenerator

An object that generates thumbnail images based on provided requirements.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
class QLThumbnailGenerator
```

## Mentioned in 

Creating Quick Look Thumbnails to Preview Files in Your App

Providing Thumbnails of Your Custom File Types

## Topics

### Getting the Generator Instance

class var shared: QLThumbnailGenerator

The singleton thumbnail generator instance.

### Generating a Thumbnail

func generateBestRepresentation(for: QLThumbnailGenerator.Request, completion: (QLThumbnailRepresentation?, (any Error)?) -> Void)

Generates the best possible thumbnail representation for a file and calls a handler upon completion.

func generateRepresentations(for: QLThumbnailGenerator.Request, update: ((QLThumbnailRepresentation?, QLThumbnailRepresentation.RepresentationType, (any Error)?) -> Void)?)

Generates various thumbnail representations for a file and calls the update handler for each thumbnail representation.

class Request

A request to generate a thumbnail for a file.

### Saving a Thumbnail

func saveBestRepresentation(for: QLThumbnailGenerator.Request, to: URL, contentType: String, completion: ((any Error)?) -> Void)

Saves the best representation of thumbnail for a specific request to the specified URL.

Deprecated

### Canceling

func cancel(QLThumbnailGenerator.Request)

Cancels the generation of a thumbnail for a given request.

### Instance Methods

func saveBestRepresentation(for: QLThumbnailGenerator.Request, to: URL, as: UTType, completion: ((any Error)?) -> Void)

Saves a thumbnail for the request on disk at fileURL. The file saved at fileURL has to be deleted when it is not used anymore. This is primarily intended for file provider extensions which need to upload thumbnails and have a small memory limit.

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

### Thumbnail Generation

Creating Quick Look Thumbnails to Preview Files in Your App

Generate thumbnails of images, text files, PDFs, audio files, videos, and more.

class QLThumbnailRepresentation

Information about the thumbnail that the thumbnail generator returns.

