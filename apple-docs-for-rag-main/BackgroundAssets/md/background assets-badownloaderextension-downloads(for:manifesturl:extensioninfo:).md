

- Background Assets
- BADownloaderExtension
-  downloads(for:manifestURL:extensionInfo:) 

Instance Method

# downloads(for:manifestURL:extensionInfo:)

iOS 16.1+iPadOS 16.1+Mac CatalystmacOS 13.0+tvOS 18.4+visionOS 2.4+

``` source
func downloads(
    for request: BAContentRequest,
    manifestURL: URL,
    extensionInfo: BAAppExtensionInfo
) -> Set
```

**Required** Default implementation provided.

## Default Implementations

### BADownloaderExtension Implementations

func downloads(for: BAContentRequest, manifestURL: URL, extensionInfo: BAAppExtensionInfo) -> Set&lt;BADownload>

Invoked by the system when the extension should check for updated content. This method will be invoked by the system upon requested events defined in `BAContentRequest`. This method should return a set of all `BAURLDownload`’s that your extension would like to schedule. During the invocation of this method, `BADownloadManager` will prohibit the ability to schedule additional downloads until this method exits scope. Therefore, all downloads needing to be scheduled should be returned here. If a download fails, it can be rescheduled using `BADownloadManager` in any other method in this protocol.

## See Also

### Checking for asset updates

enum BAContentRequest

class BAAppExtensionInfo

