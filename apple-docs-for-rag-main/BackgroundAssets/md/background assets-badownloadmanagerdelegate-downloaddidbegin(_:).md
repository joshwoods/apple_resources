

- Background Assets
- BADownloadManagerDelegate
-  downloadDidBegin(\_:) 

Instance Method

# downloadDidBegin(\_:)

Informs the delegate about a started asset download.

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 18.4+visionOS 2.4+

``` source
optional func downloadDidBegin(_ download: BADownload)
```

## Parameters 

`download`  

The started asset download.

## See Also

### Reacting to download events

func download(BADownload, didReceive: URLAuthenticationChallenge, completionHandler: (URLSession.AuthChallengeDisposition, URLCredential?) -> Void)

Tells the delegate to resolve the specified URL authentication challenge.

func download(BADownload, didWriteBytes: Int64, totalBytesWritten: Int64, totalBytesExpectedToWrite: Int64)

Informs the delegate about the progress of the specified asset download.

func downloadDidPause(BADownload)

Informs the delegate about a paused asset download.

