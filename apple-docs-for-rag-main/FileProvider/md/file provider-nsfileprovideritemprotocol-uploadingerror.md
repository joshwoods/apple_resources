

- File Provider
- NSFileProviderItemProtocol
-  uploadingError 

Instance Property

# uploadingError

An object describing an error that occurred while uploading the item.

iOS 11.0+iPadOS 11.0+macOS 11.0+visionOS 1.0+

``` source
optional var uploadingError: (any Error)? { get }
```

## Mentioned in 

Handling Errors with User-Driven Actions

## See Also

### Monitoring File Transfers

var isUploading: Bool

A Boolean value that indicates whether the item is currently uploading to your remote server.

var isUploaded: Bool

A Boolean value that indicates whether the item has been uploaded to your remote server.

var isDownloading: Bool

A Boolean value that indicates whether the item is currently downloading from your remote server.

var isDownloaded: Bool

A Boolean value that indicates whether the item has been downloaded from your remote server.

var downloadingError: (any Error)?

An object describing an error that occurred while downloading the item.

