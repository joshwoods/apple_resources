

- RealityKit
- AnimationLibraryComponent
- AnimationLibraryComponent.AnimationCollection
-  AnimationLibraryComponent.AnimationCollection.Iterator 

Structure

# AnimationLibraryComponent.AnimationCollection.Iterator

An object to iterate over all animations in the collection.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct Iterator
```

## Topics

### Instance Methods

func next() -> AnimationLibraryComponent.AnimationCollection.Element?

Advances to the next element and returns it, or `nil` if no next element exists.

### Type Aliases

typealias Element

The type of element traversed by the iterator.

## Relationships

### Conforms To

- IteratorProtocol

## See Also

### Iterating over animations

func makeIterator() -> AnimationLibraryComponent.AnimationCollection.Iterator

Returns an iterator over the animations in the collection.

