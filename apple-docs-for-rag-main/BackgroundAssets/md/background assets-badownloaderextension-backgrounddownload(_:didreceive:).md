

- Background Assets
- BADownloaderExtension
-  backgroundDownload(\_:didReceive:) 

Instance Method

# backgroundDownload(\_:didReceive:)

iOS 16.1+iPadOS 16.1+Mac CatalystmacOS 13.0+tvOS 18.4+visionOS 2.4+

``` source
func backgroundDownload(
    _ download: BADownload,
    didReceive challenge: URLAuthenticationChallenge
) async -> (URLSession.AuthChallengeDisposition, URLCredential?)
```

**Required** Default implementation provided.

## Default Implementations

### BADownloaderExtension Implementations

func backgroundDownload(BADownload, didReceive: URLAuthenticationChallenge) async -> (URLSession.AuthChallengeDisposition, URLCredential?)

Download is about to begin but requires an authentication challenge to continue.

## See Also

### Processing downloads

func backgroundDownload(BADownload, finishedWithFileURL: URL)

**Required** Default implementation provided.

func backgroundDownload(BADownload, failedWithError: any Error)

**Required** Default implementation provided.

