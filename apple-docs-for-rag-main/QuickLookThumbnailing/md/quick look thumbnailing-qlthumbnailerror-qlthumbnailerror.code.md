

- Quick Look Thumbnailing
- QLThumbnailError
-  QLThumbnailError.Code 

Enumeration

# QLThumbnailError.Code

Error codes that may be returned when generating a thumbnail.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
enum Code
```

## Topics

### Error Codes

case generationFailed

The thumbnail couldn’t be created for the given file.

case noCachedThumbnail

A low-quality thumbnail couldn’t be created.

case noCloudThumbnail

The thumbnail for a remote file couldn’t be created.

case requestCancelled

The request to create a thumbnail was canceled.

case requestInvalid

The request to create a thumbnail was invalid, for example, there’s no file at a provided URL.

case savingToURLFailed

The thumbnail couldn’t be saved at the given URL.

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

### Error Information

let QLThumbnailErrorDomain: String

The error domain of the QuickLookThumbnailing framework.

struct QLThumbnailError

Error information that might return when you generate a thumbnail.

