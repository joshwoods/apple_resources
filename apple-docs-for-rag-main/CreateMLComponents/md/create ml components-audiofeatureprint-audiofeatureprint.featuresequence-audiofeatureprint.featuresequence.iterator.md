

- Create ML Components
- AudioFeaturePrint
- AudioFeaturePrint.FeatureSequence
-  AudioFeaturePrint.FeatureSequence.Iterator 

Structure

# AudioFeaturePrint.FeatureSequence.Iterator

An async iterator of audio buffers.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
struct Iterator
```

## Topics

### Getting the next element

func next() async throws -> TemporalFeature&lt;MLShapedArray&lt;Float>>?

Asynchronously advances to the next element and returns it, or ends the sequence if there is no next element.

### Type Aliases

typealias Element

### Default Implementations

AsyncIteratorProtocol Implementations

## Relationships

### Conforms To

- AsyncIteratorProtocol

## See Also

### Creating an iterator

func makeAsyncIterator() -> AudioFeaturePrint.FeatureSequence.AsyncIterator

Constructs an iterator.

typealias AsyncIterator

The type of asynchronous iterator that produces elements of this asynchronous sequence.

typealias Feature

The feature type.

