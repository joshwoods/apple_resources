

- Create ML Components
- AudioReader
-  applied(to:eventHandler:) 

Instance Method

# applied(to:eventHandler:)

Reads an audio file as an async sequence of audio buffers.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func applied(
    to url: URL,
    eventHandler: EventHandler? = nil
) throws -> AudioReader.AsyncBuffers
```

## Parameters 

`url`  

An audio file URL.

`eventHandler`  

An event handler.

## Return Value

An async sequence of `AVAudioPCMBuffer`.

