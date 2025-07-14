

- AVFoundation
- AVAssetDownloadTask
-  loadedTimeRanges 

Instance Property

# loadedTimeRanges

The time ranges of the downloaded media that are ready for playback.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.15–11.0DeprecatedvisionOS 1.0+

``` source
var loadedTimeRanges: [NSValue] { get }
```

## Discussion

The time ranges that this property provides may be discontinuous.

## See Also

### Accessing Task Information

var urlAsset: AVURLAsset

The asset that this task downloads.

var options: [String : Any]?

The configuration options for the task.

var destinationURL: URL

The local file URL to where the task downloads the asset.

Deprecated

