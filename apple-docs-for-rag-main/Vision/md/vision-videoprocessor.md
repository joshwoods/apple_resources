

- Vision
-  VideoProcessor 

Class

# VideoProcessor

An object that performs offline analysis of video content.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
final class VideoProcessor
```

## Topics

### Creating a video processor

init(URL)

Creates a video processor to perform framework requests against the video asset you specify.

### Adding and removing a request

func addRequest&lt;T>(T, cadence: VideoProcessor.Cadence?) async throws -> some AsyncSequence&lt;T.Result, any Error> 

Adds a request to the video processor.

enum Cadence

A type that describes the video processing cadence.

func removeRequest(any VisionRequest) async -> Bool

Stops performing a request on future frames.

### Starting the analysis

func startAnalysis(of: CMTimeRange?)

Begins analyzing video frames.

### Cancelling the analysis

func cancel() async

Stops the video processor.

## Relationships

### Conforms To

- Sendable

## See Also

### Utilities

enum ComputeStage

Types that represent the compute stage.

