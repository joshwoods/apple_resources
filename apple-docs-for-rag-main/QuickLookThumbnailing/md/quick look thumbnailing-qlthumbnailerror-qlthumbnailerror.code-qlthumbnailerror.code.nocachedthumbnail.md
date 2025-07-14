

- Quick Look Thumbnailing
- QLThumbnailError
- QLThumbnailError.Code
-  QLThumbnailError.Code.noCachedThumbnail 

Case

# QLThumbnailError.Code.noCachedThumbnail

A low-quality thumbnail couldn’t be created.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
case noCachedThumbnail
```

## Discussion

In response to a request for a low-quality thumbnail, QuickLookThumbnailing searched for a previously created thumbnail to achieve a lower latency but didn’t find one.

## See Also

### Error Codes

case generationFailed

The thumbnail couldn’t be created for the given file.

case noCloudThumbnail

The thumbnail for a remote file couldn’t be created.

case requestCancelled

The request to create a thumbnail was canceled.

case requestInvalid

The request to create a thumbnail was invalid, for example, there’s no file at a provided URL.

case savingToURLFailed

The thumbnail couldn’t be saved at the given URL.

