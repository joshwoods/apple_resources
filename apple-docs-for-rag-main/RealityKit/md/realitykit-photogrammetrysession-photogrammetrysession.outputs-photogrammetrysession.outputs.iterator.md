

- RealityKit
- PhotogrammetrySession
- PhotogrammetrySession.Outputs
-  PhotogrammetrySession.Outputs.Iterator 

Structure

# PhotogrammetrySession.Outputs.Iterator

An object for iterating over published output objects.

iOS 17.0+iPadOS 17.0+Mac Catalyst 15.0+macOS 12.0+

``` source
struct Iterator
```

## Topics

### Output iteration

typealias Element

func next() async throws -> PhotogrammetrySession.Outputs.Element?

Asynchronously advances to the next element and returns it, or ends the sequence if there is no next element.

### Default Implementations

AsyncIteratorProtocol Implementations

## Relationships

### Conforms To

- AsyncIteratorProtocol

## See Also

### Iterating the collection

func makeAsyncIterator() -> PhotogrammetrySession.Outputs.Iterator

Creates an asynchronous iterator for the collection.

typealias AsyncIterator

The type of asynchronous iterator that produces elements of this asynchronous sequence.

typealias Element

The type of element used for Photogrammetry Session updates.

