

- AVFoundation
-  AVAssetDownloadTaskPrefersHDRKey 

Global Variable

# AVAssetDownloadTaskPrefersHDRKey

A key that indicates whether the task downloads HDR instead of SDR video, when available.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0–11.0DeprecatedvisionOS 1.0+

``` source
let AVAssetDownloadTaskPrefersHDRKey: String
```

## Discussion

By default, a download task prefers downloading HDR content. Provide a Boolean value of false to change this behavior.

## See Also

### Download Option Keys

let AVAssetDownloadTaskMinimumRequiredMediaBitrateKey: String

A key that indicates the minimum bit rate of the variant to download.

let AVAssetDownloadTaskMinimumRequiredPresentationSizeKey: String

A key that indicates the minimum presentation size of the variant to download.

let AVAssetDownloadTaskMediaSelectionKey: String

A key that indicates which media selection to download.

let AVAssetDownloadTaskMediaSelectionPrefersMultichannelKey: String

A key that indicates whether the task downloads media selections with support for multichannel playback, when available.

let AVAssetDownloadTaskPrefersLosslessAudioKey: String

A key that indicates whether the task downloads media selections in lossless audio format, when available.

