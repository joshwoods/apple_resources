

- Quick Look Thumbnailing
- QLThumbnailError
-  requestCancelled 

Type Property

# requestCancelled

The request to create a thumbnail was canceled.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
static var requestCancelled: QLThumbnailError.Code { get }
```

## Discussion

An app canceled a request to create a thumbnail using QLThumbnailGenerator’s cancel(_:) method.

## See Also

### Error Codes

static var generationFailed: QLThumbnailError.Code

The thumbnail couldn’t be created for the given file.

static var noCachedThumbnail: QLThumbnailError.Code

A low-quality thumbnail couldn’t be created.

static var noCloudThumbnail: QLThumbnailError.Code

The thumbnail for a remote file couldn’t be created.

static var requestInvalid: QLThumbnailError.Code

The request to create a thumbnail was invalid, for example, there’s no file at a provided URL.

static var savingToURLFailed: QLThumbnailError.Code

The thumbnail couldn’t be saved at the given URL.

enum Code

Error codes that may be returned when generating a thumbnail.

