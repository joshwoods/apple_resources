

- Vision
- VideoProcessor
-  addRequest(\_:cadence:) 

Instance Method

# addRequest(\_:cadence:)

Adds a request to the video processor.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
final func addRequest(
    _ request: T,
    cadence: VideoProcessor.Cadence? = nil
) async throws -> some AsyncSequence where T : VisionRequest
```

## Parameters 

`request`  

The request to perform.

`cadence`  

The cadency that specifies how to process the frames.

## Return Value

An AsyncSequence that produces a request result for each frame.

## Discussion

By default, the framework processes every frame.

## See Also

### Adding and removing a request

enum Cadence

A type that describes the video processing cadence.

func removeRequest(any VisionRequest) async -> Bool

Stops performing a request on future frames.

