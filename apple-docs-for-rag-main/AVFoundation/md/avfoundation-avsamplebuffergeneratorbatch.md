

- AVFoundation
-  AVSampleBufferGeneratorBatch 

Class

# AVSampleBufferGeneratorBatch

An object that generates sample buffers in a batch.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
class AVSampleBufferGeneratorBatch
```

## Overview

The benefit of batching is it aggregates adjacent I/O requests and overlaps them when possible for all sample buffers within the batch.

## Topics

### Preparing a Batch

func makeDataReady(completionHandler: ((any Error)?) -> Void)

Loads sample data asynchronously for all sample buffers within a batch.

### Canceling a Batch

func cancel()

Cancels any I/O for this batch.

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
- Sendable

## See Also

### Sample buffer generation

Playing custom audio with your own player

Construct an audio player to play your custom audio data, and optionally take advantage of the advanced features of AirPlay 2.

class AVSampleBufferRequest

An object that describes a sample buffer creation request.

class AVSampleBufferGenerator

An object that creates sample buffers.

