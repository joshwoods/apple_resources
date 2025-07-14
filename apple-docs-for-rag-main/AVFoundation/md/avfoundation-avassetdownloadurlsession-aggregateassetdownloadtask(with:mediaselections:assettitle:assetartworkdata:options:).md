

- AVFoundation
- AVAssetDownloadURLSession
-  aggregateAssetDownloadTask(with:mediaSelections:assetTitle:assetArtworkData:options:) 

Instance Method

# aggregateAssetDownloadTask(with:mediaSelections:assetTitle:assetArtworkData:options:)

Creates a download task to download the asset and media selections.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15–11.0DeprecatedvisionOS 1.0+

``` source
func aggregateAssetDownloadTask(
    with URLAsset: AVURLAsset,
    mediaSelections: [AVMediaSelection],
    assetTitle title: String,
    assetArtworkData artworkData: Data?,
    options: [String : Any]? = nil
) -> AVAggregateAssetDownloadTask?
```

## Parameters 

`URLAsset`  

The asset to download to the local device.

`mediaSelections`  

An array of media selections to download.

`title`  

A human readable title for this asset in the user’s preferred language. The system displays this value in the usage pane of the Settings app.

`artworkData`  

Optional artwork data for this asset. The system displays the image in the usage pane of the Settings app.

`options`  

Configures custom behavior on the download task.

## Return Value

An aggregate asset download task.

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

func makeAssetDownloadTask(asset: AVURLAsset, assetTitle: String, assetArtworkData: Data?, options: [String : Any]?) -> AVAssetDownloadTask?

Creates a download task to download the asset.

func makeAssetDownloadTask(asset: AVURLAsset, destinationURL: URL, options: [String : Any]?) -> AVAssetDownloadTask?

Creates a download task to download the asset to the indicated location.

Deprecated

