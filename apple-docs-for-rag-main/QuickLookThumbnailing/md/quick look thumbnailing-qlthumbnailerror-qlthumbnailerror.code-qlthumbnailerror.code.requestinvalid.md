

- Quick Look Thumbnailing
- QLThumbnailError
- QLThumbnailError.Code
-  QLThumbnailError.Code.requestInvalid 

Case

# QLThumbnailError.Code.requestInvalid

The request to create a thumbnail was invalid, for example, there’s no file at a provided URL.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
case requestInvalid
```

## See Also

### Error Codes

case generationFailed

The thumbnail couldn’t be created for the given file.

case noCachedThumbnail

A low-quality thumbnail couldn’t be created.

case noCloudThumbnail

The thumbnail for a remote file couldn’t be created.

case requestCancelled

The request to create a thumbnail was canceled.

case savingToURLFailed

The thumbnail couldn’t be saved at the given URL.

