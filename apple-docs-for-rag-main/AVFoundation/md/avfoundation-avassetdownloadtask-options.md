

- AVFoundation
- AVAssetDownloadTask
-  options 

Instance Property

# options

The configuration options for the task.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.15–11.0DeprecatedvisionOS 1.0+

``` source
var options: [String : Any]? { get }
```

## See Also

### Accessing Task Information

var urlAsset: AVURLAsset

The asset that this task downloads.

var loadedTimeRanges: [NSValue]

The time ranges of the downloaded media that are ready for playback.

var destinationURL: URL

The local file URL to where the task downloads the asset.

Deprecated

