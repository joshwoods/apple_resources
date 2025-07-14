

- Swift
- Dictionary
-  Dictionary.Index 

Structure

# Dictionary.Index

The position of a key-value pair in a dictionary.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct Index
```

Available when `Key` conforms to `Hashable`.

## Overview

Dictionary has two subscripting interfaces:

1.  Subscripting with a key, yielding an optional value:

    ```
    v = d[k]!
    ```

2.  Subscripting with an index, yielding a key-value pair:

    ```
    (k, v) = d[i]
    ```

## Topics

### Default Implementations

Comparable Implementations

Equatable Implementations

Hashable Implementations

## Relationships

### Conforms To

- Comparable

  Conforms when `Key` conforms to `Hashable`, `Value` conforms to `Copyable`, and `Value` conforms to `Escapable`.

- Copyable

  Conforms when `Key` conforms to `Hashable`, `Value` conforms to `Copyable`, and `Value` conforms to `Escapable`.

- Equatable

  Conforms when `Key` conforms to `Hashable`, `Value` conforms to `Copyable`, and `Value` conforms to `Escapable`.

- Hashable

  Conforms when `Key` conforms to `Hashable`, `Value` conforms to `Copyable`, and `Value` conforms to `Escapable`.

- Sendable

  Conforms when `Key` conforms to `Hashable`, `Key` conforms to `Sendable`, `Value` conforms to `Copyable`, `Value` conforms to `Escapable`, and `Value` conforms to `Sendable`.

## See Also

### Supporting Types

struct Keys

A view of a dictionary’s keys.

struct Values

A view of a dictionary’s values.

typealias Indices

A type that represents the indices that are valid for subscripting the collection, in ascending order.

struct Iterator

An iterator over the members of a `Dictionary`.

