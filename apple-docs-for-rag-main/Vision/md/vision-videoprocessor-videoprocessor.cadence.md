

- Vision
- VideoProcessor
-  VideoProcessor.Cadence 

Enumeration

# VideoProcessor.Cadence

A type that describes the video processing cadence.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
enum Cadence
```

## Topics

### Getting the intervals

case timeInterval(CMTime)

A cadence that processes, at most, one frame during each interval you specify.

case frameInterval(Int)

A cadence that processes every frame you specify.

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Adding and removing a request

func addRequest&lt;T>(T, cadence: VideoProcessor.Cadence?) async throws -> some AsyncSequence&lt;T.Result, any Error> 

Adds a request to the video processor.

func removeRequest(any VisionRequest) async -> Bool

Stops performing a request on future frames.

