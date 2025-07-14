

- Create ML Components
- AudioReader
-  AudioReader.MicrophoneAsyncBuffers 

Structure

# AudioReader.MicrophoneAsyncBuffers

An async sequence of audio frames.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
struct MicrophoneAsyncBuffers
```

## Overview

This sequence allows iterating through the microphone audio frames.

## Topics

### Getting the count

var count: Int?

The number of audio buffers. For this sequence count is always nil.

### Creating an iterator

func makeAsyncIterator() -> AudioReader.MicrophoneAsyncBuffers.Iterator

Constructs an iterator.

class Iterator

An async iterator of audio frames.

typealias AsyncIterator

The type of asynchronous iterator that produces elements of this asynchronous sequence.

typealias Feature

The feature type.

### Type Aliases

typealias Element

The type of element produced by this asynchronous sequence.

### Default Implementations

AsyncSequence Implementations

## Relationships

### Conforms To

- AsyncSequence
- Sendable
- TemporalSequence

## See Also

### Managing buffers

struct AsyncBuffers

An async sequence of audio buffers read from an audio file.

struct Configuration

The configuration of the audio reader.

