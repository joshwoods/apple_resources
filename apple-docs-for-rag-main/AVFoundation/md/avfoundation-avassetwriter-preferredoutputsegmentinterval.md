

- AVFoundation
- AVAssetWriter
-  preferredOutputSegmentInterval 

Instance Property

# preferredOutputSegmentInterval

The interval of output segments that you prefer.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var preferredOutputSegmentInterval: CMTime { get set }
```

## Discussion

The default value is invalid, which indicates that the asset writer chooses an appropriate default value. You may also set a positive numeric or indefinite time. When the value is indefinite, each call you make to flushSegment() outputs a segment data.

You can’t change this value after writing starts.

## See Also

### Configuring Segment Writing

var delegate: (any AVAssetWriterDelegate)?

A delegate object that responds to asset-writing events.

protocol AVAssetWriterDelegate

A delegate protocol that defines the methods to implement to respond to asset-writing events.

var initialSegmentStartTime: CMTime

The start time of the initial segment.

var outputFileTypeProfile: AVFileTypeProfile?

A profile for the output file type.

func flushSegment()

Closes the current segment and outputs it to a delegate method.

