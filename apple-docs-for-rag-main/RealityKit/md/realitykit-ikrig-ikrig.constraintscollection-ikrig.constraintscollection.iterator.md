

- RealityKit
- IKRig
- IKRig.ConstraintsCollection
-  IKRig.ConstraintsCollection.Iterator 

Structure

# IKRig.ConstraintsCollection.Iterator

A type that provides the collection’s iteration interface and encapsulates its iteration state.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct Iterator
```

## Overview

By default, a collection conforms to the `Sequence` protocol by supplying `IndexingIterator` as its associated `Iterator` type.

## Topics

### Instance Methods

func next() -> IKRig.ConstraintsCollection.Element?

Advances to the next element and returns it, or `nil` if no next element exists.

### Type Aliases

typealias Element

The type of element traversed by the iterator.

## Relationships

### Conforms To

- IteratorProtocol

