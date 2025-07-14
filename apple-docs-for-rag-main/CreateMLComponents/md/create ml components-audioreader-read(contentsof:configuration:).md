

- Create ML Components
- AudioReader
-  read(contentsOf:configuration:) 

Type Method

# read(contentsOf:configuration:)

Reads an audio file as an async sequence of audio buffers.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
static func read(
    contentsOf url: URL,
    configuration: AudioReader.Configuration = .init()
) throws -> AudioReader.AsyncBuffers
```

## Parameters 

`url`  

An audio file URL.

`configuration`  

The configuration for reading buffers.

## Return Value

An async sequence of `AVAudioPCMBuffer`.

## See Also

### Reading audio

static func read&lt;S>(S, configuration: AudioReader.Configuration) throws -> [AudioReader.AsyncBuffers]

Reads a sequence of files as an array of async sequences of audio buffers.

static func read&lt;S, Annotation>(S, configuration: AudioReader.Configuration) throws -> [AnnotatedFeature&lt;AudioReader.AsyncBuffers, Annotation>]

Reads a sequence of annotated files as a lazy sequence of results each containing an audio buffers or an error.

static func readMicrophone(configuration: AudioReader.Configuration) async throws -> AudioReader.MicrophoneAsyncBuffers

Reads an async sequence of audio frames captured with a microphone.

