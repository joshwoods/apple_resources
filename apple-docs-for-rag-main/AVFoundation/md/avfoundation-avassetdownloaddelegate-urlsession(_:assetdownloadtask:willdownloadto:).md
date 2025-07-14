

- AVFoundation
- AVAssetDownloadDelegate
-  urlSession(\_:assetDownloadTask:willDownloadTo:) 

Instance Method

# urlSession(\_:assetDownloadTask:willDownloadTo:)

Tells the delegate when a download task determines its download location.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 14.0+visionOS 1.0+watchOS 10.0+

``` source
optional func urlSession(
    _ session: URLSession,
    assetDownloadTask: AVAssetDownloadTask,
    willDownloadTo location: URL
)
```

## Parameters 

`session`  

The session the asset download task is on.

`assetDownloadTask`  

The download task.

`location`  

The URL the task downloads the asset to.

## Discussion

Save the returned URL to instantiate the asset in the future.

## See Also

### Responding to Download Events

func urlSession(URLSession, assetDownloadTask: AVAssetDownloadTask, didResolve: AVMediaSelection)

Tells the delegate that a download task resolved the media selection to download, including any automatic selections.

func urlSession(URLSession, assetDownloadTask: AVAssetDownloadTask, didLoad: CMTimeRange, totalTimeRangesLoaded: [NSValue], timeRangeExpectedToLoad: CMTimeRange)

Tells the delegate that a download task loaded a new time range.

func urlSession(URLSession, assetDownloadTask: AVAssetDownloadTask, didFinishDownloadingTo: URL)

Tells the delegate that a download task finished downloading the requested asset.

func urlSession(URLSession, assetDownloadTask: AVAssetDownloadTask, willDownloadVariants: [AVAssetVariant])

Tells the delegate that a download task completed variant selection.

