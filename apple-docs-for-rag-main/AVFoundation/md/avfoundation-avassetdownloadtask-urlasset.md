

- AVFoundation
- AVAssetDownloadTask
-  urlAsset 

Instance Property

# urlAsset

The asset that this task downloads.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+watchOS 10.0+

``` source
var urlAsset: AVURLAsset { get }
```

## See Also

### Accessing Task Information

var loadedTimeRanges: [NSValue]

The time ranges of the downloaded media that are ready for playback.

var options: [String : Any]?

The configuration options for the task.

var destinationURL: URL

The local file URL to where the task downloads the asset.

Deprecated

