

- AVFoundation
-  AVAssetDownloadTaskMediaSelectionKey 

Global Variable

# AVAssetDownloadTaskMediaSelectionKey

A key that indicates which media selection to download.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.15–11.0DeprecatedvisionOS 1.0+

``` source
let AVAssetDownloadTaskMediaSelectionKey: String
```

## Discussion

By default, a download task automatically retrieves all of an asset’s media selections. To download a specific media selection, provide an AVMediaSelection object for this key.

## See Also

### Download Option Keys

let AVAssetDownloadTaskMinimumRequiredMediaBitrateKey: String

A key that indicates the minimum bit rate of the variant to download.

let AVAssetDownloadTaskMinimumRequiredPresentationSizeKey: String

A key that indicates the minimum presentation size of the variant to download.

let AVAssetDownloadTaskMediaSelectionPrefersMultichannelKey: String

A key that indicates whether the task downloads media selections with support for multichannel playback, when available.

let AVAssetDownloadTaskPrefersHDRKey: String

A key that indicates whether the task downloads HDR instead of SDR video, when available.

let AVAssetDownloadTaskPrefersLosslessAudioKey: String

A key that indicates whether the task downloads media selections in lossless audio format, when available.

