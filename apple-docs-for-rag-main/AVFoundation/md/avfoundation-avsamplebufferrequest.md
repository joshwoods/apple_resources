

- AVFoundation
-  AVSampleBufferRequest 

Class

# AVSampleBufferRequest

An object that describes a sample buffer creation request.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 10.10+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
class AVSampleBufferRequest
```

## Topics

### Creating a Request

init(start: AVSampleCursor)

Creates a newly allocated sample buffer request with the specified sample cursor.

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

var startCursor: AVSampleCursor

The starting cursor position.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Sample buffer generation

Playing custom audio with your own player

Construct an audio player to play your custom audio data, and optionally take advantage of the advanced features of AirPlay 2.

class AVSampleBufferGenerator

An object that creates sample buffers.

class AVSampleBufferGeneratorBatch

An object that generates sample buffers in a batch.

