

- AVFoundation
-  AVAssetDownloadTaskMinimumRequiredPresentationSizeKey 

Global Variable

# AVAssetDownloadTaskMinimumRequiredPresentationSizeKey

A key that indicates the minimum presentation size of the variant to download.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0–11.0DeprecatedvisionOS 1.0+

``` source
let AVAssetDownloadTaskMinimumRequiredPresentationSizeKey: String
```

## Discussion

By default, a download task selects the variant with the largest media presentation size. To download a variant of a particular size, provide a CGSize value for this key.

## See Also

### Download Option Keys

let AVAssetDownloadTaskMinimumRequiredMediaBitrateKey: String

A key that indicates the minimum bit rate of the variant to download.

let AVAssetDownloadTaskMediaSelectionKey: String

A key that indicates which media selection to download.

let AVAssetDownloadTaskMediaSelectionPrefersMultichannelKey: String

A key that indicates whether the task downloads media selections with support for multichannel playback, when available.

let AVAssetDownloadTaskPrefersHDRKey: String

A key that indicates whether the task downloads HDR instead of SDR video, when available.

let AVAssetDownloadTaskPrefersLosslessAudioKey: String

A key that indicates whether the task downloads media selections in lossless audio format, when available.

