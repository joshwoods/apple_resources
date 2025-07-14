

- Vision
- VideoProcessor
-  removeRequest(\_:) 

Instance Method

# removeRequest(\_:)

Stops performing a request on future frames.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
final func removeRequest(_ request: any VisionRequest) async -> Bool
```

## Parameters 

`request`  

The request to remove.

## See Also

### Adding and removing a request

func addRequest&lt;T>(T, cadence: VideoProcessor.Cadence?) async throws -> some AsyncSequence&lt;T.Result, any Error> 

Adds a request to the video processor.

enum Cadence

A type that describes the video processing cadence.

