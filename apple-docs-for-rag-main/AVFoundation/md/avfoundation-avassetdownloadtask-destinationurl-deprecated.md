

- AVFoundation
- AVAssetDownloadTask
-  destinationURL Deprecated

Instance Property

# destinationURL

The local file URL to where the task downloads the asset.

iOS 9.0–10.0DeprecatediPadOS 9.0–10.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
var destinationURL: URL { get }
```

Deprecated

Use the URL property of URLAsset instead

## See Also

### Accessing Task Information

var urlAsset: AVURLAsset

The asset that this task downloads.

var loadedTimeRanges: [NSValue]

The time ranges of the downloaded media that are ready for playback.

var options: [String : Any]?

The configuration options for the task.

