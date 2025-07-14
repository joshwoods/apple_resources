

- AVFoundation
- AVAssetWriter
-  flushSegment() 

Instance Method

# flushSegment()

Closes the current segment and outputs it to a delegate method.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func flushSegment()
```

## Discussion

Call this method only when the preferredOutputSegmentInterval property value is indefinite.

## See Also

### Configuring Segment Writing

var delegate: (any AVAssetWriterDelegate)?

A delegate object that responds to asset-writing events.

protocol AVAssetWriterDelegate

A delegate protocol that defines the methods to implement to respond to asset-writing events.

var preferredOutputSegmentInterval: CMTime

The interval of output segments that you prefer.

var initialSegmentStartTime: CMTime

The start time of the initial segment.

var outputFileTypeProfile: AVFileTypeProfile?

A profile for the output file type.

