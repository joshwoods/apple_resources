

- Quick Look Thumbnailing
- QLThumbnailError
- QLThumbnailError.Code
-  QLThumbnailError.Code.requestCancelled 

Case

# QLThumbnailError.Code.requestCancelled

The request to create a thumbnail was canceled.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
case requestCancelled
```

## Discussion

An app canceled a request to create a thumbnail using QLThumbnailGenerator’s cancel(_:) method.

## See Also

### Error Codes

case generationFailed

The thumbnail couldn’t be created for the given file.

case noCachedThumbnail

A low-quality thumbnail couldn’t be created.

case noCloudThumbnail

The thumbnail for a remote file couldn’t be created.

case requestInvalid

The request to create a thumbnail was invalid, for example, there’s no file at a provided URL.

case savingToURLFailed

The thumbnail couldn’t be saved at the given URL.

