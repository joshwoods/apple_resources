

- AVFoundation
-  AVAssetDownloadURLSession 

Class

# AVAssetDownloadURLSession

A URL session that creates and executes asset download tasks.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+watchOS 10.0+

``` source
class AVAssetDownloadURLSession
```

## Topics

### Creating a Download Session

init(configuration: URLSessionConfiguration, assetDownloadDelegate: (any AVAssetDownloadDelegate)?, delegateQueue: OperationQueue?)

Creates a URL session to download assets.

protocol AVAssetDownloadDelegate

A protocol that defines the methods to implement to respond to asset-download events.

### Creating Download Tasks

func makeAssetDownloadTask(downloadConfiguration: AVAssetDownloadConfiguration) -> AVAssetDownloadTask

Creates a download task that uses the specified configuration.

class AVAssetDownloadConfiguration

An object that provides the configuration for a download task.

func makeAssetDownloadTask(asset: AVURLAsset, assetTitle: String, assetArtworkData: Data?, options: [String : Any]?) -> AVAssetDownloadTask?

Creates a download task to download the asset.

func aggregateAssetDownloadTask(with: AVURLAsset, mediaSelections: [AVMediaSelection], assetTitle: String, assetArtworkData: Data?, options: [String : Any]?) -> AVAggregateAssetDownloadTask?

Creates a download task to download the asset and media selections.

func makeAssetDownloadTask(asset: AVURLAsset, destinationURL: URL, options: [String : Any]?) -> AVAssetDownloadTask?

Creates a download task to download the asset to the indicated location.

Deprecated

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

## Relationships

### Inherits From

- URLSession

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Asset downloading

Using AVFoundation to play and persist HTTP Live Streams

Play HTTP Live Streams and persist streams on disk for offline playback using AVFoundation.

class AVAssetDownloadTask

A session used to download HTTP Live Streaming assets.

class AVAggregateAssetDownloadTask

A task that downloads multiple media selections for an asset.

