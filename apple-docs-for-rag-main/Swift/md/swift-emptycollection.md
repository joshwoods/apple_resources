

- Swift
-  EmptyCollection 

Structure

# EmptyCollection

A collection whose element type is `Element` but that is always empty.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct EmptyCollection
```

## Topics

### Initializers

init()

Creates an instance.

### Default Implementations

BidirectionalCollection Implementations

Collection Implementations

Equatable Implementations

MutableCollection Implementations

RandomAccessCollection Implementations

Sequence Implementations

## Relationships

### Conforms To

- BidirectionalCollection

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- BitwiseCopyable

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- Collection

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- ContiguousBytes
- Copyable

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- DataProtocol
- Equatable

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- MutableCollection

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- RandomAccessCollection

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- Sendable

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- Sequence

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

## See Also

### Special-Use Collections

func repeatElement&lt;T>(T, count: Int) -> Repeated&lt;T>

Creates a collection containing the specified number of the given element.

struct CollectionOfOne

A collection containing a single element.

struct KeyValuePairs

A lightweight collection of key-value pairs.

typealias DictionaryLiteral

