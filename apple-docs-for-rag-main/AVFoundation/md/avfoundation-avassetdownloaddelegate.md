

- AVFoundation
-  AVAssetDownloadDelegate 

Protocol

# AVAssetDownloadDelegate

A protocol that defines the methods to implement to respond to asset-download events.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+watchOS 10.0+

``` source
protocol AVAssetDownloadDelegate : URLSessionTaskDelegate
```

## Topics

### Responding to Download Events

func urlSession(URLSession, assetDownloadTask: AVAssetDownloadTask, didResolve: AVMediaSelection)

Tells the delegate that a download task resolved the media selection to download, including any automatic selections.

func urlSession(URLSession, assetDownloadTask: AVAssetDownloadTask, didLoad: CMTimeRange, totalTimeRangesLoaded: [NSValue], timeRangeExpectedToLoad: CMTimeRange)

Tells the delegate that a download task loaded a new time range.

func urlSession(URLSession, assetDownloadTask: AVAssetDownloadTask, didFinishDownloadingTo: URL)

Tells the delegate that a download task finished downloading the requested asset.

func urlSession(URLSession, assetDownloadTask: AVAssetDownloadTask, willDownloadVariants: [AVAssetVariant])

Tells the delegate that a download task completed variant selection.

func urlSession(URLSession, assetDownloadTask: AVAssetDownloadTask, willDownloadTo: URL)

Tells the delegate when a download task determines its download location.

### Responding to Aggregate Download Events

func urlSession(URLSession, aggregateAssetDownloadTask: AVAggregateAssetDownloadTask, willDownloadTo: URL)

Tells the delegate the final location of the asset when the download completes.

func urlSession(URLSession, aggregateAssetDownloadTask: AVAggregateAssetDownloadTask, didLoad: CMTimeRange, totalTimeRangesLoaded: [NSValue], timeRangeExpectedToLoad: CMTimeRange, for: AVMediaSelection)

Tells the delegate that the aggregate download task loaded a new time range.

func urlSession(URLSession, aggregateAssetDownloadTask: AVAggregateAssetDownloadTask, didCompleteFor: AVMediaSelection)

Tells the delegate that a child task finished downloading a media selection.

## Relationships

### Inherits From

- NSObjectProtocol
- Sendable
- URLSessionDelegate
- URLSessionTaskDelegate

## See Also

### Creating a Download Session

init(configuration: URLSessionConfiguration, assetDownloadDelegate: (any AVAssetDownloadDelegate)?, delegateQueue: OperationQueue?)

Creates a URL session to download assets.

