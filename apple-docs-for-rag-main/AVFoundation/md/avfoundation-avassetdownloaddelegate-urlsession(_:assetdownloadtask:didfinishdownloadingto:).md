

- AVFoundation
- AVAssetDownloadDelegate
-  urlSession(\_:assetDownloadTask:didFinishDownloadingTo:) 

Instance Method

# urlSession(\_:assetDownloadTask:didFinishDownloadingTo:)

Tells the delegate that a download task finished downloading the requested asset.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15–11.0DeprecatedvisionOS 1.0+watchOS 10.0–11.4Deprecated

``` source
optional func urlSession(
    _ session: URLSession,
    assetDownloadTask: AVAssetDownloadTask,
    didFinishDownloadingTo location: URL
)
```

## Parameters 

`session`  

The session the asset download task is on.

`assetDownloadTask`  

The download task whose downloaded completed.

`location`  

The download location of the asset.

## Discussion

Don’t move the downloaded asset from this location. Downloaded assets must remain at the system-provided URL. Instead, save a persistent reference to this URL for future use.

## See Also

### Responding to Download Events

func urlSession(URLSession, assetDownloadTask: AVAssetDownloadTask, didResolve: AVMediaSelection)

Tells the delegate that a download task resolved the media selection to download, including any automatic selections.

func urlSession(URLSession, assetDownloadTask: AVAssetDownloadTask, didLoad: CMTimeRange, totalTimeRangesLoaded: [NSValue], timeRangeExpectedToLoad: CMTimeRange)

Tells the delegate that a download task loaded a new time range.

func urlSession(URLSession, assetDownloadTask: AVAssetDownloadTask, willDownloadVariants: [AVAssetVariant])

Tells the delegate that a download task completed variant selection.

func urlSession(URLSession, assetDownloadTask: AVAssetDownloadTask, willDownloadTo: URL)

Tells the delegate when a download task determines its download location.

