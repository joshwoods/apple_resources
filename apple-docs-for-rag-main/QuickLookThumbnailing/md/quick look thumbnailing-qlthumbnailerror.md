

- Quick Look Thumbnailing
-  QLThumbnailError 

Structure

# QLThumbnailError

Error information that might return when you generate a thumbnail.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
struct QLThumbnailError
```

## Topics

### Error Codes

static var generationFailed: QLThumbnailError.Code

The thumbnail couldn’t be created for the given file.

static var noCachedThumbnail: QLThumbnailError.Code

A low-quality thumbnail couldn’t be created.

static var noCloudThumbnail: QLThumbnailError.Code

The thumbnail for a remote file couldn’t be created.

static var requestCancelled: QLThumbnailError.Code

The request to create a thumbnail was canceled.

static var requestInvalid: QLThumbnailError.Code

The request to create a thumbnail was invalid, for example, there’s no file at a provided URL.

static var savingToURLFailed: QLThumbnailError.Code

The thumbnail couldn’t be saved at the given URL.

enum Code

Error codes that may be returned when generating a thumbnail.

### Type Properties

static var errorDomain: String

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Error Information

let QLThumbnailErrorDomain: String

The error domain of the QuickLookThumbnailing framework.

enum Code

Error codes that may be returned when generating a thumbnail.

