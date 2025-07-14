

- File Provider
- NSFileProviderItemProtocol
-  isDownloaded 

Instance Property

# isDownloaded

A Boolean value that indicates whether the item has been downloaded from your remote server.

iOS 11.0+iPadOS 11.0+macOS 11.0+visionOS 1.0+

``` source
optional var isDownloaded: Bool { get }
```

## See Also

### Monitoring File Transfers

var isUploading: Bool

A Boolean value that indicates whether the item is currently uploading to your remote server.

var isUploaded: Bool

A Boolean value that indicates whether the item has been uploaded to your remote server.

var uploadingError: (any Error)?

An object describing an error that occurred while uploading the item.

var isDownloading: Bool

A Boolean value that indicates whether the item is currently downloading from your remote server.

var downloadingError: (any Error)?

An object describing an error that occurred while downloading the item.

