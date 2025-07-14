

- Background Assets
- BADownloaderExtension
-  backgroundDownload(\_:failedWithError:) 

Instance Method

# backgroundDownload(\_:failedWithError:)

iOS 16.1+iPadOS 16.1+Mac CatalystmacOS 13.0+tvOS 18.4+visionOS 2.4+

``` source
func backgroundDownload(
    _ failedDownload: BADownload,
    failedWithError error: any Error
)
```

**Required** Default implementation provided.

## Default Implementations

### BADownloaderExtension Implementations

func backgroundDownload(BADownload, failedWithError: any Error)

This method is called when a download has failed but there is no `BADownloadManager` delegate to handle the completion event. When a download has failed, this method will be invoked. If a download fails you may reschedule it with `BADownloadManager`.

## See Also

### Processing downloads

func backgroundDownload(BADownload, didReceive: URLAuthenticationChallenge) async -> (URLSession.AuthChallengeDisposition, URLCredential?)

**Required** Default implementation provided.

func backgroundDownload(BADownload, finishedWithFileURL: URL)

**Required** Default implementation provided.

