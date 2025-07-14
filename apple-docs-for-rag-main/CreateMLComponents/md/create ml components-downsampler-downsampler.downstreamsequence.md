

- Create ML Components
- Downsampler
-  Downsampler.DownStreamSequence 

Structure

# Downsampler.DownStreamSequence

An async sequence of down stream elements.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct DownStreamSequence
```

Available when `Input` conforms to `Sendable`.

## Topics

### Getting the count

var count: Int?

The count of elements.

### Creating an iterator

func makeAsyncIterator() -> Downsampler&lt;Input>.DownStreamSequence.Iterator

Creates the asynchronous iterator that produces elements of this asynchronous sequence.

struct Iterator

An async iterator of down stream sequence.

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

### Performing the transformation

func applied&lt;S>(to: S, eventHandler: EventHandler?) throws -> Downsampler&lt;Input>.DownStreamSequence

Down samples the input sequence

typealias Input

The input type.

typealias Output

The output type.

