

- Background Assets
-  BADownloadManagerDelegate 

Protocol

# BADownloadManagerDelegate

An interface for reacting to asset download events and processing concluded downloads.

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 18.4+visionOS 2.4+

``` source
protocol BADownloadManagerDelegate : NSObjectProtocol
```

## Topics

### Reacting to download events

func downloadDidBegin(BADownload)

Informs the delegate about a started asset download.

func download(BADownload, didReceive: URLAuthenticationChallenge, completionHandler: (URLSession.AuthChallengeDisposition, URLCredential?) -> Void)

Tells the delegate to resolve the specified URL authentication challenge.

func download(BADownload, didWriteBytes: Int64, totalBytesWritten: Int64, totalBytesExpectedToWrite: Int64)

Informs the delegate about the progress of the specified asset download.

func downloadDidPause(BADownload)

Informs the delegate about a paused asset download.

### Processing concluded downloads

func download(BADownload, finishedWithFileURL: URL)

Informs the delegate about a finished asset download and provides the on-disk location.

func download(BADownload, failedWithError: any Error)

Informs the delegate about a failed asset download.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Monitoring downloads

var delegate: (any BADownloadManagerDelegate)?

The download manager’s delegate.

