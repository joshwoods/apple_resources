

- BrowserEngineKit
- BEDownloadMonitor
-  resumeMonitoring(placeholderURL:) 

Instance Method

# resumeMonitoring(placeholderURL:)

Informs the system that it needs to resume monitoring the download.

iOS 18.2+iPadOS 18.2+

``` source
@objc(resumeMonitoring:completionHandler:)
func resumeMonitoring(placeholderURL: URL) async throws
```

## Parameters 

`placeholderURL`  

The placeholder location your networking extension previously received when it called beginMonitoring().

## Discussion

Call this method when your browser resumes the download after an interruption, for example, someone cancels the download, or your networking extension encounters a network error.

## See Also

### Reporting progress to the system

func beginMonitoring() async throws -> BEDownloadMonitor.Location?

Informs the system to start monitoring the download.

