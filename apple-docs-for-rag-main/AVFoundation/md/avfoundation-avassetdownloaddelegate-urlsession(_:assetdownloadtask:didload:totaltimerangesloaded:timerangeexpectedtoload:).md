

- AVFoundation
- AVAssetDownloadDelegate
-  urlSession(\_:assetDownloadTask:didLoad:totalTimeRangesLoaded:timeRangeExpectedToLoad:) 

Instance Method

# urlSession(\_:assetDownloadTask:didLoad:totalTimeRangesLoaded:timeRangeExpectedToLoad:)

Tells the delegate that a download task loaded a new time range.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.15–11.0DeprecatedvisionOS 1.0+

``` source
optional func urlSession(
    _ session: URLSession,
    assetDownloadTask: AVAssetDownloadTask,
    didLoad timeRange: CMTimeRange,
    totalTimeRangesLoaded loadedTimeRanges: [NSValue],
    timeRangeExpectedToLoad: CMTimeRange
)
```

## Parameters 

`session`  

The session the asset download task is on.

`assetDownloadTask`  

The download task that loaded a new time range.

`timeRange`  

A CMTimeRange value that indicates the time range the task loaded since the last call to this method.

`loadedTimeRanges`  

An array of CMTimeRange values that indicate the time ranges the task has downloaded so far.

`timeRangeExpectedToLoad`  

A CMTimeRange value that indicates the expected duration of the downloaded asset.

## Discussion

Implement this method to track the download status of an asset. The following example shows how to calculate the percentage complete for the current download.

- Swift
- Objective-C

```
func urlSession(_ session: URLSession, assetDownloadTask: AVAssetDownloadTask, didLoad timeRange: CMTimeRange, totalTimeRangesLoaded loadedTimeRanges: [NSValue], timeRangeExpectedToLoad: CMTimeRange) {
    var percentageComplete = 0.0
    // Iterate over loaded time ranges
    for value in loadedTimeRanges {
        // Unpack CMTimeRange value
        let loadedTimeRange = value.timeRangeValue
        percentageComplete += loadedTimeRange.duration.seconds / timeRangeExpectedToLoad.duration.seconds
    }
    percentageComplete *= 100
    // Updated interested observers of percentage change
}
```

```
- (void)URLSession:(NSURLSession *)session assetDownloadTask:(AVAssetDownloadTask *)assetDownloadTask
                                            didLoadTimeRange:(CMTimeRange)timeRange
                                       totalTimeRangesLoaded:(NSArray *)loadedTimeRanges
                                     timeRangeExpectedToLoad:(CMTimeRange)timeRangeExpectedToLoad {
    double percentageComplete = 0.0f;
    // Iterate over loaded time ranges
    for (NSValue *value in loadedTimeRanges) {
        // Unpack CMTimeRange value
        CMTimeRange loadedTimeRange = value.CMTimeRangeValue;
        percentageComplete +=
            CMTimeGetSeconds(loadedTimeRange.duration) / CMTimeGetSeconds(timeRangeExpectedToLoad.duration);
    }
    percentageComplete *= 100;
    // Updated interested observers of percentage change
}
```

## See Also

### Responding to Download Events

func urlSession(URLSession, assetDownloadTask: AVAssetDownloadTask, didResolve: AVMediaSelection)

Tells the delegate that a download task resolved the media selection to download, including any automatic selections.

func urlSession(URLSession, assetDownloadTask: AVAssetDownloadTask, didFinishDownloadingTo: URL)

Tells the delegate that a download task finished downloading the requested asset.

func urlSession(URLSession, assetDownloadTask: AVAssetDownloadTask, willDownloadVariants: [AVAssetVariant])

Tells the delegate that a download task completed variant selection.

func urlSession(URLSession, assetDownloadTask: AVAssetDownloadTask, willDownloadTo: URL)

Tells the delegate when a download task determines its download location.

