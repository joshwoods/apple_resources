

- Create ML Components
- PreprocessedFeatureSequence
-  PreprocessedFeatureSequence.AsyncIterator 

Structure

# PreprocessedFeatureSequence.AsyncIterator

The type of asynchronous iterator that produces elements of this asynchronous sequence.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct AsyncIterator
```

## Topics

### Getting the next element

func next() -> TemporalFeature&lt;Feature>?

Asynchronously advances to the next element and returns it, or ends the sequence if there is no next element.

### Type Aliases

typealias Element

### Default Implementations

AsyncIteratorProtocol Implementations

## Relationships

### Conforms To

- AsyncIteratorProtocol

