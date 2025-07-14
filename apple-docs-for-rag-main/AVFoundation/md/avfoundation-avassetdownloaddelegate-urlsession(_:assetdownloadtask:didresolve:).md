

- AVFoundation
- AVAssetDownloadDelegate
-  urlSession(\_:assetDownloadTask:didResolve:) 

Instance Method

# urlSession(\_:assetDownloadTask:didResolve:)

Tells the delegate that a download task resolved the media selection to download, including any automatic selections.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
optional func urlSession(
    _ session: URLSession,
    assetDownloadTask: AVAssetDownloadTask,
    didResolve resolvedMediaSelection: AVMediaSelection
)
```

## Parameters 

`session`  

The session the asset download task is on.

`assetDownloadTask`  

The task that resolved the media selection.

`resolvedMediaSelection`  

The media selection the task resolved.

## Discussion

For the best chance of playing back downloaded content without further network I/O, set this selection on the associated AVPlayerItem.

## See Also

### Responding to Download Events

func urlSession(URLSession, assetDownloadTask: AVAssetDownloadTask, didLoad: CMTimeRange, totalTimeRangesLoaded: [NSValue], timeRangeExpectedToLoad: CMTimeRange)

Tells the delegate that a download task loaded a new time range.

func urlSession(URLSession, assetDownloadTask: AVAssetDownloadTask, didFinishDownloadingTo: URL)

Tells the delegate that a download task finished downloading the requested asset.

func urlSession(URLSession, assetDownloadTask: AVAssetDownloadTask, willDownloadVariants: [AVAssetVariant])

Tells the delegate that a download task completed variant selection.

func urlSession(URLSession, assetDownloadTask: AVAssetDownloadTask, willDownloadTo: URL)

Tells the delegate when a download task determines its download location.

