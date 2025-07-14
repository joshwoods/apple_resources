

- Create ML Components
- AudioReader
-  AudioReader.Configuration 

Structure

# AudioReader.Configuration

The configuration of the audio reader.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
struct Configuration
```

## Topics

### Creating a configuration

init()

Creates an AudioReader Configuration

init(frameCount: Int)

Creates an AudioReader Configuration

### Getting the frame count

var frameCount: Int

The maximum size of each buffer in frames. The default value is `4096`.

## Relationships

### Conforms To

- Sendable

## See Also

### Managing buffers

struct AsyncBuffers

An async sequence of audio buffers read from an audio file.

struct MicrophoneAsyncBuffers

An async sequence of audio frames.

