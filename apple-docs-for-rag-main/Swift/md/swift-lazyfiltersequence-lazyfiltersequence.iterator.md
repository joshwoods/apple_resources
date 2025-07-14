

- Swift
- LazyFilterSequence
-  LazyFilterSequence.Iterator 

Structure

# LazyFilterSequence.Iterator

An iterator over the elements traversed by some base iterator that also satisfy a given predicate.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct Iterator
```

Available when `Base` conforms to `Sequence`.

## Overview

Note

This is the associated `Iterator` of `LazyFilterSequence` and `LazyFilterCollection`.

## Topics

### Instance Properties

var base: Base.Iterator

The underlying iterator whose elements are being filtered.

### Default Implementations

IteratorProtocol Implementations

Sequence Implementations

## Relationships

### Conforms To

- Copyable

  Conforms when `Base` conforms to `Sequence`.

- IteratorProtocol

  Conforms when `Base` conforms to `Sequence`.

- Sequence

  Conforms when `Base` conforms to `Sequence`.

