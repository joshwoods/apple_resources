

- Swift
- Dictionary
-  Dictionary.Iterator 

Structure

# Dictionary.Iterator

An iterator over the members of a `Dictionary`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct Iterator
```

Available when `Key` conforms to `Hashable`.

## Topics

### Default Implementations

CustomReflectable Implementations

IteratorProtocol Implementations

## Relationships

### Conforms To

- Copyable

  Conforms when `Key` conforms to `Hashable`, `Value` conforms to `Copyable`, and `Value` conforms to `Escapable`.

- CustomReflectable

  Conforms when `Key` conforms to `Hashable`, `Value` conforms to `Copyable`, and `Value` conforms to `Escapable`.

- IteratorProtocol

  Conforms when `Key` conforms to `Hashable`, `Value` conforms to `Copyable`, and `Value` conforms to `Escapable`.

- Sendable

  Conforms when `Key` conforms to `Hashable`, `Key` conforms to `Sendable`, `Value` conforms to `Copyable`, `Value` conforms to `Escapable`, and `Value` conforms to `Sendable`.

## See Also

### Supporting Types

struct Keys

A view of a dictionary’s keys.

struct Values

A view of a dictionary’s values.

struct Index

The position of a key-value pair in a dictionary.

typealias Indices

A type that represents the indices that are valid for subscripting the collection, in ascending order.

