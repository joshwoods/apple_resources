

- Swift
- Set
-  Set.Index 

Structure

# Set.Index

The position of an element in a set.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct Index
```

Available when `Element` conforms to `Hashable`.

## Topics

### Default Implementations

Comparable Implementations

Equatable Implementations

Hashable Implementations

## Relationships

### Conforms To

- Comparable

  Conforms when `Element` conforms to `Hashable`.

- Copyable

  Conforms when `Element` conforms to `Hashable`.

- Equatable

  Conforms when `Element` conforms to `Hashable`.

- Hashable

  Conforms when `Element` conforms to `Hashable`.

- Sendable

  Conforms when `Element` conforms to `Hashable` and `Sendable`.

## See Also

### Supporting Types

struct Iterator

An iterator over the members of a `Set`.

