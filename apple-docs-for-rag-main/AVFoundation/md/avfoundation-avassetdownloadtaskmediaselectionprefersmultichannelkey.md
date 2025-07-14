

- AVFoundation
-  AVAssetDownloadTaskMediaSelectionPrefersMultichannelKey 

Global Variable

# AVAssetDownloadTaskMediaSelectionPrefersMultichannelKey

A key that indicates whether the task downloads media selections with support for multichannel playback, when available.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15–11.0DeprecatedvisionOS 1.0+

``` source
let AVAssetDownloadTaskMediaSelectionPrefersMultichannelKey: String
```

## Discussion

By default, download tasks retrieve the variant’s stereo audio and the most capable multichannel rendition available. Provide a Boolean value of false to disable this behavior.

## See Also

### Download Option Keys

let AVAssetDownloadTaskMinimumRequiredMediaBitrateKey: String

A key that indicates the minimum bit rate of the variant to download.

let AVAssetDownloadTaskMinimumRequiredPresentationSizeKey: String

A key that indicates the minimum presentation size of the variant to download.

let AVAssetDownloadTaskMediaSelectionKey: String

A key that indicates which media selection to download.

let AVAssetDownloadTaskPrefersHDRKey: String

A key that indicates whether the task downloads HDR instead of SDR video, when available.

let AVAssetDownloadTaskPrefersLosslessAudioKey: String

A key that indicates whether the task downloads media selections in lossless audio format, when available.

