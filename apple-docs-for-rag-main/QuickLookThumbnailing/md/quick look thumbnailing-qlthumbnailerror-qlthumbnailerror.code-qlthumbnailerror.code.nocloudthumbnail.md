

- Quick Look Thumbnailing
- QLThumbnailError
- QLThumbnailError.Code
-  QLThumbnailError.Code.noCloudThumbnail 

Case

# QLThumbnailError.Code.noCloudThumbnail

The thumbnail for a remote file couldn’t be created.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
case noCloudThumbnail
```

## Discussion

The creation of a thumbnail for a remote file stored in a FileProvider extension such as iCloud or another cloud service failed. The request to generate a thumbnail failed because the remote file itself isn’t available locally or couldn’t be used to generate a thumbnail. QuickLookThumbnailing tried to download a thumbnail from the cloud service instead but no thumbnail was available in the cloud service, or an available thumbnail couldn’t be downloaded.

## See Also

### Error Codes

case generationFailed

The thumbnail couldn’t be created for the given file.

case noCachedThumbnail

A low-quality thumbnail couldn’t be created.

case requestCancelled

The request to create a thumbnail was canceled.

case requestInvalid

The request to create a thumbnail was invalid, for example, there’s no file at a provided URL.

case savingToURLFailed

The thumbnail couldn’t be saved at the given URL.

