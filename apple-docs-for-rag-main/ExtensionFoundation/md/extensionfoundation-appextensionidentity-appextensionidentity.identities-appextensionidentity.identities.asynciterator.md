

- ExtensionFoundation
- AppExtensionIdentity
- AppExtensionIdentity.Identities
-  AppExtensionIdentity.Identities.AsyncIterator 

Structure

# AppExtensionIdentity.Identities.AsyncIterator

The type of the asynchronous iterator created by this asynchronous sequence.

macOS 13.0+

``` source
struct AsyncIterator
```

## Topics

### Iterating Extensions

typealias Element

The type of element produced by this asynchronous sequence.

func next() async -> [AppExtensionIdentity]?

Asynchronously advances to the next element and returns it.

## Relationships

### Conforms To

- AsyncIteratorProtocol

## See Also

### Iterating the Sequence

func next() async -> [AppExtensionIdentity]?

Asynchronously advances to the next element and returns it.

typealias Element

The type of element produced by this asynchronous sequence.

func makeAsyncIterator() -> AppExtensionIdentity.Identities.AsyncIterator

Creates the asynchronous iterator that produces elements of this asynchronous sequence.

