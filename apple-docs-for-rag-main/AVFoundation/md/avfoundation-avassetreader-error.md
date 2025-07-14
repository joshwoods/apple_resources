

- AVFoundation
- AVAssetReader
-  error 

Instance Property

# error

An error that describes the reason for a failure.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
var error: (any Error)? { get }
```

## Discussion

The value is `nil` if the asset reader’s status isn’t AVAssetReader.Status.failed.

This property is thread safe.

## See Also

### Configuring Reading

var timeRange: CMTimeRange

The time range within the asset to read.

var status: AVAssetReader.Status

The status of reading sample buffers from the asset.

enum Status

Values that represent the possible states of an asset reader.

