

- AVFoundation
- AVAssetDownloadURLSession
-  makeAssetDownloadTask(asset:assetTitle:assetArtworkData:options:) 

Instance Method

# makeAssetDownloadTask(asset:assetTitle:assetArtworkData:options:)

Creates a download task to download the asset.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15–11.0DeprecatedvisionOS 1.0+

``` source
func makeAssetDownloadTask(
    asset URLAsset: AVURLAsset,
    assetTitle title: String,
    assetArtworkData artworkData: Data?,
    options: [String : Any]? = nil
) -> AVAssetDownloadTask?
```

## Parameters 

`URLAsset`  

The HTTP Live Streaming asset to download.

`title`  

A human readable title for this asset in the user’s preferred language. The system displays this value in the usage pane of the Settings app.

`artworkData`  

Optional artwork data for this asset. The system displays the image in the usage pane of the Settings app.

`options`  

Configures custom behavior on the download task. You must provide an options dictionary to download nondefault media selections for HLS assets.

## Return Value

A new download task.

## Discussion

This method may return `nil` if you call it on an invalidated session.

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

func aggregateAssetDownloadTask(with: AVURLAsset, mediaSelections: [AVMediaSelection], assetTitle: String, assetArtworkData: Data?, options: [String : Any]?) -> AVAggregateAssetDownloadTask?

Creates a download task to download the asset and media selections.

func makeAssetDownloadTask(asset: AVURLAsset, destinationURL: URL, options: [String : Any]?) -> AVAssetDownloadTask?

Creates a download task to download the asset to the indicated location.

Deprecated

