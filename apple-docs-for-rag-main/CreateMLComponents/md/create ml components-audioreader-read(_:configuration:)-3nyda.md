

- Create ML Components
- AudioReader
-  read(\_:configuration:) 

Type Method

# read(\_:configuration:)

Reads a sequence of files as an array of async sequences of audio buffers.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
static func read(
    _ files: S,
    configuration: AudioReader.Configuration = .init()
) throws -> [AudioReader.AsyncBuffers] where S : Sequence, S.Element == URL
```

## Parameters 

`files`  

A sequence of URLs.

`configuration`  

The configuration for reading buffers.

## Return Value

An array of async sequences of audio buffers.

## See Also

### Reading audio

static func read(contentsOf: URL, configuration: AudioReader.Configuration) throws -> AudioReader.AsyncBuffers

Reads an audio file as an async sequence of audio buffers.

static func read&lt;S, Annotation>(S, configuration: AudioReader.Configuration) throws -> [AnnotatedFeature&lt;AudioReader.AsyncBuffers, Annotation>]

Reads a sequence of annotated files as a lazy sequence of results each containing an audio buffers or an error.

static func readMicrophone(configuration: AudioReader.Configuration) async throws -> AudioReader.MicrophoneAsyncBuffers

Reads an async sequence of audio frames captured with a microphone.

