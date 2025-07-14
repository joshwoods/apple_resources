

- AVFoundation
- AVAssetDownloadURLSession
-  makeAssetDownloadTask(downloadConfiguration:) 

Instance Method

# makeAssetDownloadTask(downloadConfiguration:)

Creates a download task that uses the specified configuration.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+watchOS 8.0+

``` source
func makeAssetDownloadTask(downloadConfiguration: AVAssetDownloadConfiguration) -> AVAssetDownloadTask
```

## Parameters 

`downloadConfiguration`  

The configuration that the task uses.

## Return Value

A new download task.

## Discussion

This method raises an exception if you call it on an invalidated session.

## See Also

### Creating Download Tasks

class AVAssetDownloadConfiguration

An object that provides the configuration for a download task.

func makeAssetDownloadTask(asset: AVURLAsset, assetTitle: String, assetArtworkData: Data?, options: [String : Any]?) -> AVAssetDownloadTask?

Creates a download task to download the asset.

func aggregateAssetDownloadTask(with: AVURLAsset, mediaSelections: [AVMediaSelection], assetTitle: String, assetArtworkData: Data?, options: [String : Any]?) -> AVAggregateAssetDownloadTask?

Creates a download task to download the asset and media selections.

func makeAssetDownloadTask(asset: AVURLAsset, destinationURL: URL, options: [String : Any]?) -> AVAssetDownloadTask?

Creates a download task to download the asset to the indicated location.

Deprecated

