

- AVFoundation
- AVAssetReader
-  status 

Instance Property

# status

The status of reading sample buffers from the asset.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
var status: AVAssetReader.Status { get }
```

## Discussion

Check the value of this property when the copyNextSampleBuffer() method on AVAssetReaderOutput returns `nil` to determine why the output can’t read more data.

This property is thread safe.

## See Also

### Configuring Reading

var timeRange: CMTimeRange

The time range within the asset to read.

enum Status

Values that represent the possible states of an asset reader.

var error: (any Error)?

An error that describes the reason for a failure.

