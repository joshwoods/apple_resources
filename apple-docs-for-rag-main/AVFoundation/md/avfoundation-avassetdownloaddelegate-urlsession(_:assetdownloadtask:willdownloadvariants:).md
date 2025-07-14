

- AVFoundation
- AVAssetDownloadDelegate
-  urlSession(\_:assetDownloadTask:willDownloadVariants:) 

Instance Method

# urlSession(\_:assetDownloadTask:willDownloadVariants:)

Tells the delegate that a download task completed variant selection.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+watchOS 10.0+

``` source
optional func urlSession(
    _ session: URLSession,
    assetDownloadTask: AVAssetDownloadTask,
    willDownloadVariants variants: [AVAssetVariant]
)
```

## Parameters 

`session`  

The session the asset download task is on.

`assetDownloadTask`  

The task that finished selecting variant selection.

`variants`  

The asset variants to download.

## See Also

### Responding to Download Events

func urlSession(URLSession, assetDownloadTask: AVAssetDownloadTask, didResolve: AVMediaSelection)

Tells the delegate that a download task resolved the media selection to download, including any automatic selections.

func urlSession(URLSession, assetDownloadTask: AVAssetDownloadTask, didLoad: CMTimeRange, totalTimeRangesLoaded: [NSValue], timeRangeExpectedToLoad: CMTimeRange)

Tells the delegate that a download task loaded a new time range.

func urlSession(URLSession, assetDownloadTask: AVAssetDownloadTask, didFinishDownloadingTo: URL)

Tells the delegate that a download task finished downloading the requested asset.

func urlSession(URLSession, assetDownloadTask: AVAssetDownloadTask, willDownloadTo: URL)

Tells the delegate when a download task determines its download location.

