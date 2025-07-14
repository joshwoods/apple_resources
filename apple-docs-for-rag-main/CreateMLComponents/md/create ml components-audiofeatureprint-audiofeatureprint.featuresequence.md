

- Create ML Components
- AudioFeaturePrint
-  AudioFeaturePrint.FeatureSequence 

Structure

# AudioFeaturePrint.FeatureSequence

An async sequence of audio buffers.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
struct FeatureSequence
```

## Topics

### Getting the count

var count: Int?

The number of elements in the sequence. For this sequence count is always nil.

### Creating an iterator

func makeAsyncIterator() -> AudioFeaturePrint.FeatureSequence.AsyncIterator

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

### Performing the transformation

func applied&lt;S>(to: S, eventHandler: EventHandler?) throws -> AudioFeaturePrint.FeatureSequence

Extracts audio features from an a sequence of audio buffers

func applied&lt;S, TS, Annotation>(to: S, eventHandler: EventHandler?) async throws -> [AnnotatedFeature&lt;Self.OutputSequence, Annotation>]

Performs the transformation on a sequence of annotated input sequences.

typealias Input

The input type.

typealias Output

The output type.

