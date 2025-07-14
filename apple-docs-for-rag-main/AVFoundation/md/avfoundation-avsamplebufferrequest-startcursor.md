

- AVFoundation
- AVSampleBufferRequest
-  startCursor 

Instance Property

# startCursor

The starting cursor position.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 10.10+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var startCursor: AVSampleCursor { get }
```

## Discussion

The CMSampleBuffer created with the request must include the sample at this position.

## See Also

### Configuring Sample Buffer Request Parameters

var direction: AVSampleBufferRequest.Direction

The buffer sample direction.

enum Direction

The modes that describe the buffer request direction.

var limitCursor: AVSampleCursor?

The limiting position for sample loading.

var maxSampleCount: Int

The maximum number of samples to load.

var mode: AVSampleBufferRequest.Mode

The sample buffer request mode.

enum Mode

The modes in which a sample buffer generator processes a request.

var overrideTime: CMTime

The deadline for sample data and output PTS for the sample buffer.

var preferredMinSampleCount: Int

The preferred minimum number of samples to load.

