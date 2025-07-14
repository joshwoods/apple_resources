

- AVFoundation
- AVAssetWriter
-  delegate 

Instance Property

# delegate

A delegate object that responds to asset-writing events.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
weak var delegate: (any AVAssetWriterDelegate)? { get set }
```

## See Also

### Configuring Segment Writing

protocol AVAssetWriterDelegate

A delegate protocol that defines the methods to implement to respond to asset-writing events.

var preferredOutputSegmentInterval: CMTime

The interval of output segments that you prefer.

var initialSegmentStartTime: CMTime

The start time of the initial segment.

var outputFileTypeProfile: AVFileTypeProfile?

A profile for the output file type.

func flushSegment()

Closes the current segment and outputs it to a delegate method.

