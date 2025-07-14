

- AVFoundation
-  AVAssetDownloadTaskPrefersLosslessAudioKey 

Global Variable

# AVAssetDownloadTaskPrefersLosslessAudioKey

A key that indicates whether the task downloads media selections in lossless audio format, when available.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 11.3–11.0DeprecatedvisionOS 1.0+

``` source
let AVAssetDownloadTaskPrefersLosslessAudioKey: String
```

## Discussion

By default, a download task prefers downloading lossy audio formats. Provide a Boolean value of true to change this behavior.

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

let AVAssetDownloadTaskPrefersHDRKey: String

A key that indicates whether the task downloads HDR instead of SDR video, when available.

