

- Translation
- TranslationSession
- TranslationSession.BatchResponse
-  TranslationSession.BatchResponse.AsyncIterator 

Structure

# TranslationSession.BatchResponse.AsyncIterator

The type of asynchronous iterator that produces elements of this asynchronous sequence.

iOS 18.0+iPadOS 18.0+macOS 15.0+

``` source
struct AsyncIterator
```

## Topics

### Instance Methods

func next() async throws -> TranslationSession.BatchResponse.Element?

Asynchronously advances to the next element and returns it, or ends the sequence if there is no next element.

### Type Aliases

typealias Element

### Default Implementations

AsyncIteratorProtocol Implementations

## Relationships

### Conforms To

- AsyncIteratorProtocol

