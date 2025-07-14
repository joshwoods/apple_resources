

- AVFoundation
-  AVAssetDownloadTask 

Class

# AVAssetDownloadTask

A session used to download HTTP Live Streaming assets.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+watchOS 10.0+

``` source
class AVAssetDownloadTask
```

## Overview

This class is a subclass of URLSessionTask that you use to download HTTP Live Streaming assets. You create instances of this class by calling makeAssetDownloadTask(downloadConfiguration:) on the download session.

## Topics

### Accessing Task Information

var urlAsset: AVURLAsset

The asset that this task downloads.

var loadedTimeRanges: [NSValue]

The time ranges of the downloaded media that are ready for playback.

var options: [String : Any]?

The configuration options for the task.

var destinationURL: URL

The local file URL to where the task downloads the asset.

Deprecated

## Relationships

### Inherits From

- URLSessionTask

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol
- ProgressReporting
- Sendable

## See Also

### Asset downloading

Using AVFoundation to play and persist HTTP Live Streams

Play HTTP Live Streams and persist streams on disk for offline playback using AVFoundation.

class AVAssetDownloadURLSession

A URL session that creates and executes asset download tasks.

class AVAggregateAssetDownloadTask

A task that downloads multiple media selections for an asset.

