

- AVFoundation
-  AVAssetDownloadConfiguration 

Class

# AVAssetDownloadConfiguration

An object that provides the configuration for a download task.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 10.0+

``` source
class AVAssetDownloadConfiguration
```

## Topics

### Creating a Configuration

convenience init(asset: AVURLAsset, title: String)

Creates a download configuration for a media asset.

### Accessing Configuration Details

var artworkData: Data?

A data value that represents the asset’s artwork.

var primaryContentConfiguration: AVAssetDownloadContentConfiguration

The configuration for the primary content that the task downloads.

var auxiliaryContentConfigurations: [AVAssetDownloadContentConfiguration]

The configuration for the auxiliary content that the task downloads.

class AVAssetDownloadContentConfiguration

A configuration object that contains variant qualifiers and media options.

var optimizesAuxiliaryContentConfigurations: Bool

A Boolean value that indicates whether the task optimizes auxiliary content selection.

### Instance Methods

func setInterstitialMediaSelectionCriteria([AVPlayerMediaSelectionCriteria], forMediaCharacteristic: AVMediaCharacteristic)

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Creating Download Tasks

func makeAssetDownloadTask(downloadConfiguration: AVAssetDownloadConfiguration) -> AVAssetDownloadTask

Creates a download task that uses the specified configuration.

func makeAssetDownloadTask(asset: AVURLAsset, assetTitle: String, assetArtworkData: Data?, options: [String : Any]?) -> AVAssetDownloadTask?

Creates a download task to download the asset.

func aggregateAssetDownloadTask(with: AVURLAsset, mediaSelections: [AVMediaSelection], assetTitle: String, assetArtworkData: Data?, options: [String : Any]?) -> AVAggregateAssetDownloadTask?

Creates a download task to download the asset and media selections.

func makeAssetDownloadTask(asset: AVURLAsset, destinationURL: URL, options: [String : Any]?) -> AVAssetDownloadTask?

Creates a download task to download the asset to the indicated location.

Deprecated

