

- AVFoundation
- AVAssetDownloadDelegate
-  urlSession(\_:aggregateAssetDownloadTask:willDownloadTo:) 

Instance Method

# urlSession(\_:aggregateAssetDownloadTask:willDownloadTo:)

Tells the delegate the final location of the asset when the download completes.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15–11.0DeprecatedvisionOS 1.0+

``` source
optional func urlSession(
    _ session: URLSession,
    aggregateAssetDownloadTask: AVAggregateAssetDownloadTask,
    willDownloadTo location: URL
)
```

## Parameters 

`session`  

The session the asset download task is on.

`aggregateAssetDownloadTask`  

The task that downloads the asset.

`location`  

The file URL to which the task downloads media.

## See Also

### Responding to Aggregate Download Events

func urlSession(URLSession, aggregateAssetDownloadTask: AVAggregateAssetDownloadTask, didLoad: CMTimeRange, totalTimeRangesLoaded: [NSValue], timeRangeExpectedToLoad: CMTimeRange, for: AVMediaSelection)

Tells the delegate that the aggregate download task loaded a new time range.

func urlSession(URLSession, aggregateAssetDownloadTask: AVAggregateAssetDownloadTask, didCompleteFor: AVMediaSelection)

Tells the delegate that a child task finished downloading a media selection.

