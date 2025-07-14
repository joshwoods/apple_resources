

- AVFoundation
-  AVAggregateAssetDownloadTask 

Class

# AVAggregateAssetDownloadTask

A task that downloads multiple media selections for an asset.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15–11.0DeprecatedvisionOS 1.0+

``` source
class AVAggregateAssetDownloadTask
```

## Topics

### Accessing the Asset

var urlAsset: AVURLAsset

The asset the parent task downloads.

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

class AVAssetDownloadTask

A session used to download HTTP Live Streaming assets.

