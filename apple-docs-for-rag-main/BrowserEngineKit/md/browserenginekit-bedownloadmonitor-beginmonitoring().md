

- BrowserEngineKit
- BEDownloadMonitor
-  beginMonitoring() 

Instance Method

# beginMonitoring()

Informs the system to start monitoring the download.

iOS 18.2+iPadOS 18.2+

``` source
@objc(beginMonitoring:)
func beginMonitoring() async throws -> BEDownloadMonitor.Location?
```

## Return Value

If you called useDownloadsFolder(placeholderType:finalFileCreatedHandler:), this method returns the placeholder location that the system creates to host the downloaded content; otherwise, it returns `nil`.

## Mentioned in 

Downloading files in a web browser with an alternative browser engine

## See Also

### Reporting progress to the system

func resumeMonitoring(placeholderURL: URL) async throws

Informs the system that it needs to resume monitoring the download.

