

- AVFoundation
- AVAssetDownloadDelegate
-  urlSession(\_:aggregateAssetDownloadTask:didCompleteFor:) 

Instance Method

# urlSession(\_:aggregateAssetDownloadTask:didCompleteFor:)

Tells the delegate that a child task finished downloading a media selection.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15–11.0DeprecatedvisionOS 1.0+

``` source
optional func urlSession(
    _ session: URLSession,
    aggregateAssetDownloadTask: AVAggregateAssetDownloadTask,
    didCompleteFor mediaSelection: AVMediaSelection
)
```

## Parameters 

`session`  

The session the asset download task is on.

`aggregateAssetDownloadTask`  

The download task that finished downloading the media selection.

`mediaSelection`  

The downloaded media selection.

## See Also

### Responding to Aggregate Download Events

func urlSession(URLSession, aggregateAssetDownloadTask: AVAggregateAssetDownloadTask, willDownloadTo: URL)

Tells the delegate the final location of the asset when the download completes.

func urlSession(URLSession, aggregateAssetDownloadTask: AVAggregateAssetDownloadTask, didLoad: CMTimeRange, totalTimeRangesLoaded: [NSValue], timeRangeExpectedToLoad: CMTimeRange, for: AVMediaSelection)

Tells the delegate that the aggregate download task loaded a new time range.

