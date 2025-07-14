

- AVFoundation
- AVAssetDownloadURLSession
-  makeAssetDownloadTask(asset:destinationURL:options:) Deprecated

Instance Method

# makeAssetDownloadTask(asset:destinationURL:options:)

Creates a download task to download the asset to the indicated location.

iOS 9.0–10.0DeprecatediPadOS 9.0–10.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
func makeAssetDownloadTask(
    asset URLAsset: AVURLAsset,
    destinationURL: URL,
    options: [String : Any]? = nil
) -> AVAssetDownloadTask?
```

Deprecated

Use makeAssetDownloadTask(asset:assetTitle:assetArtworkData:options:) instead.

## Parameters 

`URLAsset`  

The asset to download to the local device.

`destinationURL`  

The local file URL to download the asset to.

`options`  

Configures non-default behavior for the download task. To download nondefault media selections, you must indicate download options.

## Return Value

A new download task.

## Topics

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

let AVAssetDownloadTaskPrefersLosslessAudioKey: String

A key that indicates whether the task downloads media selections in lossless audio format, when available.

## See Also

### Creating Download Tasks

func makeAssetDownloadTask(downloadConfiguration: AVAssetDownloadConfiguration) -> AVAssetDownloadTask

Creates a download task that uses the specified configuration.

class AVAssetDownloadConfiguration

An object that provides the configuration for a download task.

func makeAssetDownloadTask(asset: AVURLAsset, assetTitle: String, assetArtworkData: Data?, options: [String : Any]?) -> AVAssetDownloadTask?

Creates a download task to download the asset.

func aggregateAssetDownloadTask(with: AVURLAsset, mediaSelections: [AVMediaSelection], assetTitle: String, assetArtworkData: Data?, options: [String : Any]?) -> AVAggregateAssetDownloadTask?

Creates a download task to download the asset and media selections.

