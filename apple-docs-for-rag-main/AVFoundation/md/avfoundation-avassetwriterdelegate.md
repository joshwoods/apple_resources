

- AVFoundation
-  AVAssetWriterDelegate 

Protocol

# AVAssetWriterDelegate

A delegate protocol that defines the methods to implement to respond to asset-writing events.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
protocol AVAssetWriterDelegate : NSObjectProtocol, Sendable
```

## Topics

### Responding to Segment Output

func assetWriter(AVAssetWriter, didOutputSegmentData: Data, segmentType: AVAssetSegmentType)

Tells the delegate that the asset writer output segment data.

func assetWriter(AVAssetWriter, didOutputSegmentData: Data, segmentType: AVAssetSegmentType, segmentReport: AVAssetSegmentReport?)

Tells the delegate that the asset writer output segment data and a report.

class AVAssetSegmentReport

An object that provides information about segment data.

## Relationships

### Inherits From

- NSObjectProtocol
- Sendable

## See Also

### Configuring Segment Writing

var delegate: (any AVAssetWriterDelegate)?

A delegate object that responds to asset-writing events.

var preferredOutputSegmentInterval: CMTime

The interval of output segments that you prefer.

var initialSegmentStartTime: CMTime

The start time of the initial segment.

var outputFileTypeProfile: AVFileTypeProfile?

A profile for the output file type.

func flushSegment()

Closes the current segment and outputs it to a delegate method.

