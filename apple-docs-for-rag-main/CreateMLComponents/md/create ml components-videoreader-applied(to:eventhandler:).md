

- Create ML Components
- VideoReader
-  applied(to:eventHandler:) 

Instance Method

# applied(to:eventHandler:)

Reads a video file as an async sequence of video frames.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func applied(
    to url: URL,
    eventHandler: EventHandler?
) async throws -> VideoReader.AsyncFrames
```

## Parameters 

`url`  

A video file URL.

`eventHandler`  

An event handler.

## Return Value

An async sequence of `VideoFrames`.

