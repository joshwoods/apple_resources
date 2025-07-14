

- AVFoundation
-  AVSampleBufferGenerator 

Class

# AVSampleBufferGenerator

An object that creates sample buffers.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 10.10+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
class AVSampleBufferGenerator
```

## Overview

Each request for `CMSampleBuffer` creation is described in an `AVSampleBufferRequest` object. The CMSampleBuffer opaque objects are returned synchronously. If requested, sample data may be loaded asynchronously (depending on file format support).

## Topics

### Creating Sample Buffer Generators

init(asset: AVAsset, timebase: CMTimebase?)

Creates a new sample buffer generator.

### Creating a Sample Buffer

func makeSampleBuffer(for: AVSampleBufferRequest) throws -> CMSampleBuffer

Creates a sample buffer, and attempts to load its data asynchronously if requested.

func makeBatch() -> AVSampleBufferGeneratorBatch

Creates a batch object to handle generating multiple sample buffers.

func makeSampleBuffer(for: AVSampleBufferRequest, addTo: AVSampleBufferGeneratorBatch) throws -> CMSampleBuffer

Creates a sample buffer and attempts to defer I/O for its data.

func createSampleBuffer(for: AVSampleBufferRequest) -> CMSampleBuffer?

Creates a new sample buffer reference for the specified buffer request.

Deprecated

### Retrieving Sample Buffer Data

class func notifyOfDataReady(for: CMSampleBuffer, completionHandler: (Bool, (any Error)?) -> Void)

Notifies the sample buffer generator when data is ready for the sample buffer reference or an error has occurred.

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

class AVSampleBufferGeneratorBatch

An object that generates sample buffers in a batch.

