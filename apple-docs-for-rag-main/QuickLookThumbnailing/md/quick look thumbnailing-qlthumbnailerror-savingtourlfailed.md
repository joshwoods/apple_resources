

- Quick Look Thumbnailing
- QLThumbnailError
-  savingToURLFailed 

Type Property

# savingToURLFailed

The thumbnail couldn’t be saved at the given URL.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
static var savingToURLFailed: QLThumbnailError.Code { get }
```

## See Also

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

enum Code

Error codes that may be returned when generating a thumbnail.

