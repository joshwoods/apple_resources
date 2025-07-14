

- Create ML Components
- AudioReader
-  readMicrophone(configuration:) 

Type Method

# readMicrophone(configuration:)

Reads an async sequence of audio frames captured with a microphone.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
static func readMicrophone(configuration: AudioReader.Configuration = .init()) async throws -> AudioReader.MicrophoneAsyncBuffers
```

## Parameters 

`configuration`  

The configuration for reading buffers.

## Return Value

An async sequence of `AVAudioPCMBuffer`.

## See Also

### Reading audio

static func read(contentsOf: URL, configuration: AudioReader.Configuration) throws -> AudioReader.AsyncBuffers

Reads an audio file as an async sequence of audio buffers.

static func read&lt;S>(S, configuration: AudioReader.Configuration) throws -> [AudioReader.AsyncBuffers]

Reads a sequence of files as an array of async sequences of audio buffers.

static func read&lt;S, Annotation>(S, configuration: AudioReader.Configuration) throws -> [AnnotatedFeature&lt;AudioReader.AsyncBuffers, Annotation>]

Reads a sequence of annotated files as a lazy sequence of results each containing an audio buffers or an error.

