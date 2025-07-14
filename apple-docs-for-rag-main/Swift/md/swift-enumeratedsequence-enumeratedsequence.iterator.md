

- Swift
- EnumeratedSequence
-  EnumeratedSequence.Iterator 

Structure

# EnumeratedSequence.Iterator

The iterator for `EnumeratedSequence`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct Iterator
```

Available when `Base` conforms to `Sequence`.

## Overview

An instance of this iterator wraps a base iterator and yields successive `Int` values, starting at zero, along with the elements of the underlying base iterator. The following example enumerates the elements of an array:

```
var iterator = ["foo", "bar"].enumerated().makeIterator()
iterator.next() // (0, "foo")
iterator.next() // (1, "bar")
iterator.next() // nil
```

To create an instance, call `enumerated().makeIterator()` on a sequence or collection.

## Topics

### Default Implementations

IteratorProtocol Implementations

Sequence Implementations

## Relationships

### Conforms To

- Copyable

  Conforms when `Base` conforms to `Sequence`.

- IteratorProtocol

  Conforms when `Base` conforms to `Sequence`.

- Sendable

  Conforms when `Base` conforms to `Sequence` and `Base.Iterator` conforms to `Sendable`.

- Sequence

  Conforms when `Base` conforms to `Sequence`.

