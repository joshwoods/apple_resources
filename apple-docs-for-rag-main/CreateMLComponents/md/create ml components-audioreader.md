

- Create ML Components
-  AudioReader 

Structure

# AudioReader

An audio file reader.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
struct AudioReader
```

## Topics

### Creating an audio reader

init(configuration: AudioReader.Configuration)

Creates an audio reader.

### Getting the properties

var configuration: AudioReader.Configuration

The audio reader configuration

### Managing buffers

struct AsyncBuffers

An async sequence of audio buffers read from an audio file.

struct Configuration

The configuration of the audio reader.

struct MicrophoneAsyncBuffers

An async sequence of audio frames.

### Reading audio

static func read(contentsOf: URL, configuration: AudioReader.Configuration) throws -> AudioReader.AsyncBuffers

Reads an audio file as an async sequence of audio buffers.

static func read&lt;S>(S, configuration: AudioReader.Configuration) throws -> [AudioReader.AsyncBuffers]

Reads a sequence of files as an array of async sequences of audio buffers.

static func read&lt;S, Annotation>(S, configuration: AudioReader.Configuration) throws -> [AnnotatedFeature&lt;AudioReader.AsyncBuffers, Annotation>]

Reads a sequence of annotated files as a lazy sequence of results each containing an audio buffers or an error.

static func readMicrophone(configuration: AudioReader.Configuration) async throws -> AudioReader.MicrophoneAsyncBuffers

Reads an async sequence of audio frames captured with a microphone.

### Applying

func applied(to: URL, eventHandler: EventHandler?) throws -> AudioReader.AsyncBuffers

Reads an audio file as an async sequence of audio buffers.

### Type Aliases

typealias Input

The input type.

typealias Output

The output type.

### Default Implementations

Transformer Implementations

## Relationships

### Conforms To

- Sendable
- Transformer

## See Also

### Audio components

struct AudioFeaturePrint

A stream transformer that extracts audio features from audio buffers.

struct AudioConvertingTransformer

A transformer for audio conversion.

