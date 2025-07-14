

- Background Assets
- BADownloadManagerDelegate
-  download(\_:didWriteBytes:totalBytesWritten:totalBytesExpectedToWrite:) 

Instance Method

# download(\_:didWriteBytes:totalBytesWritten:totalBytesExpectedToWrite:)

Informs the delegate about the progress of the specified asset download.

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 18.4+visionOS 2.4+

``` source
optional func download(
    _ download: BADownload,
    didWriteBytes bytesWritten: Int64,
    totalBytesWritten: Int64,
    totalBytesExpectedToWrite totalExpectedBytes: Int64
)
```

## Parameters 

`download`  

The associated asset download.

`bytesWritten`  

The number of bytes the system writes to disk for the asset download since the previous execution of this method.

`totalBytesWritten`  

The total number of bytes the system writes to disk for the asset download.

`totalExpectedBytes`  

The total size, in bytes, that the framework expects to receive for the asset download.

## Discussion

Because the framework may be processing several asset downloads at once, it may call this method frequently and for different downloads. Cache an asset download’s uniqueIdentifier when you first schedule it, and then match the identifier against the same property on `download` so you can track the individual progress of all in-progress downloads.

## See Also

### Reacting to download events

func downloadDidBegin(BADownload)

Informs the delegate about a started asset download.

func download(BADownload, didReceive: URLAuthenticationChallenge, completionHandler: (URLSession.AuthChallengeDisposition, URLCredential?) -> Void)

Tells the delegate to resolve the specified URL authentication challenge.

func downloadDidPause(BADownload)

Informs the delegate about a paused asset download.

