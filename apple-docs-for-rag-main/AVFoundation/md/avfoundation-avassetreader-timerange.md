

- AVFoundation
- AVAssetReader
-  timeRange 

Instance Property

# timeRange

The time range within the asset to read.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
var timeRange: CMTimeRange { get set }
```

## Discussion

The default value is a time range with a start time of zero and a duration of positiveInfinity.

You can’t modify this value after reading starts.

## See Also

### Configuring Reading

var status: AVAssetReader.Status

The status of reading sample buffers from the asset.

enum Status

Values that represent the possible states of an asset reader.

var error: (any Error)?

An error that describes the reason for a failure.

