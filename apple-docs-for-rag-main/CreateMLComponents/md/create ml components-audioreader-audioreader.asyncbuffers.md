

- Create ML Components
- AudioReader
-  AudioReader.AsyncBuffers 

Structure

# AudioReader.AsyncBuffers

An async sequence of audio buffers read from an audio file.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
struct AsyncBuffers
```

## Overview

This sequence allows iterating through the file only once.

## Topics

### Getting the count

let count: Int?

The number of audio buffers in the file.

### Getting the url

let url: URL

The audio file URL, used when throwing an error.

### Creating an iterator

func makeAsyncIterator() -> AudioReader.AsyncBuffers.Iterator

Constructs an iterator.

struct Iterator

An async iterator of audio buffers.

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
- TemporalSequence

## See Also

### Managing buffers

struct Configuration

The configuration of the audio reader.

struct MicrophoneAsyncBuffers

An async sequence of audio frames.

