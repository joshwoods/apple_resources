

- Create ML Components
- HumanBodyActionCounter
-  HumanBodyActionCounter.CumulativeSumSequence 

Structure

# HumanBodyActionCounter.CumulativeSumSequence

Cumulative human body action count sequence.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
struct CumulativeSumSequence
```

## Topics

### Getting the count

var count: Int?

The estimated number of predictions.

### Creating an iterator

func makeAsyncIterator() -> HumanBodyActionCounter.CumulativeSumSequence.Iterator

Constructs an iterator.

struct Iterator

An async iterator of cumulative count sequence.

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

func applied&lt;S>(to: S, eventHandler: EventHandler?) async throws -> HumanBodyActionCounter.OutputSequence

Predicts cumulative human body action counts from a sequence of human body pose windows.

typealias Input

The input type.

typealias Output

The output type.

typealias OutputSequence

The output async sequence type.

