

- Background Assets
- BADownloadManager
-  fetchCurrentDownloads() 

Instance Method

# fetchCurrentDownloads()

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 18.4+visionOS 2.4+

``` source
func fetchCurrentDownloads() throws -> [BADownload]
```

## See Also

### Fetching in-progress downloads

func fetchCurrentDownloads(completionHandler: ([BADownload], (any Error)?) -> Void)

Fetches the contents of the manager’s download queue.

