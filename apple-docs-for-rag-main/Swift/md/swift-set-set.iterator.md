

- Swift
- Set
-  Set.Iterator 

Structure

# Set.Iterator

An iterator over the members of a `Set`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct Iterator
```

Available when `Element` conforms to `Hashable`.

## Topics

### Default Implementations

CustomReflectable Implementations

IteratorProtocol Implementations

## Relationships

### Conforms To

- Copyable

  Conforms when `Element` conforms to `Hashable`.

- CustomReflectable

  Conforms when `Element` conforms to `Hashable`.

- IteratorProtocol

  Conforms when `Element` conforms to `Hashable`.

- Sendable

  Conforms when `Element` conforms to `Hashable` and `Sendable`.

## See Also

### Supporting Types

struct Index

The position of an element in a set.

