

- Swift
-  CollectionOfOne 

Structure

# CollectionOfOne

A collection containing a single element.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct CollectionOfOne
```

## Overview

You can use a `CollectionOfOne` instance when you need to efficiently represent a single value as a collection. For example, you can add a single element to an array by using a `CollectionOfOne` instance with the concatenation operator (`+`):

```
let a = [1, 2, 3, 4]
let toAdd = 100
let b = a + CollectionOfOne(toAdd)
// b == [1, 2, 3, 4, 100]
```

## Topics

### Initializers

init(Element)

Creates an instance containing just the given element.

### Default Implementations

BidirectionalCollection Implementations

Collection Implementations

CustomDebugStringConvertible Implementations

CustomReflectable Implementations

MutableCollection Implementations

RandomAccessCollection Implementations

Sequence Implementations

## Relationships

### Conforms To

- BidirectionalCollection

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- Collection

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- ContiguousBytes
- Copyable

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- CustomDebugStringConvertible

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- CustomReflectable

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- MutableCollection

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- RandomAccessCollection

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- Sendable

  Conforms when `Element` conforms to `Copyable`, `Escapable`, and `Sendable`.

- Sequence

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

## See Also

### Special-Use Collections

func repeatElement&lt;T>(T, count: Int) -> Repeated&lt;T>

Creates a collection containing the specified number of the given element.

struct EmptyCollection

A collection whose element type is `Element` but that is always empty.

struct KeyValuePairs

A lightweight collection of key-value pairs.

typealias DictionaryLiteral

