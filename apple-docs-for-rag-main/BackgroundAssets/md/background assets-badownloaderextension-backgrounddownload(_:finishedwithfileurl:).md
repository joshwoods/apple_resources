

- Background Assets
- BADownloaderExtension
-  backgroundDownload(\_:finishedWithFileURL:) 

Instance Method

# backgroundDownload(\_:finishedWithFileURL:)

iOS 16.1+iPadOS 16.1+Mac CatalystmacOS 13.0+tvOS 18.4+visionOS 2.4+

``` source
func backgroundDownload(
    _ finishedDownload: BADownload,
    finishedWithFileURL fileURL: URL
)
```

**Required** Default implementation provided.

## Default Implementations

### BADownloaderExtension Implementations

func backgroundDownload(BADownload, finishedWithFileURL: URL)

This method is called when a download has finished but there is no `BADownloadManager` delegate to handle the completion event.

## See Also

### Processing downloads

func backgroundDownload(BADownload, didReceive: URLAuthenticationChallenge) async -> (URLSession.AuthChallengeDisposition, URLCredential?)

**Required** Default implementation provided.

func backgroundDownload(BADownload, failedWithError: any Error)

**Required** Default implementation provided.

