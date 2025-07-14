

- RealityKit
- UnsafeForceEffectBuffer
-  UnsafeForceEffectBuffer.Iterator 

Structure

# UnsafeForceEffectBuffer.Iterator

Iterates over all elements of the `UnsafeForceEffectBuffer`.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct Iterator
```

## Topics

### Instance Methods

func next() -> T?

Advances to the next element and returns it, or `nil` if no next element exists.

### Type Aliases

typealias Element

The type of element traversed by the iterator.

## Relationships

### Conforms To

- IteratorProtocol

