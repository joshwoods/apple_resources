

- Swift
- ReversedCollection
-  ReversedCollection.Index 

Structure

# ReversedCollection.Index

An index that traverses the same positions as an underlying index, with inverted traversal direction.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct Index
```

Available when `Base` conforms to `BidirectionalCollection`.

## Topics

### Initializers

init(Base.Index)

Creates a new index into a reversed collection for the position before the specified index.

### Instance Properties

let base: Base.Index

The position after this position in the underlying collection.

### Default Implementations

Comparable Implementations

Equatable Implementations

Hashable Implementations

## Relationships

### Conforms To

- Comparable

  Conforms when `Base` conforms to `BidirectionalCollection`.

- Copyable

  Conforms when `Base` conforms to `BidirectionalCollection` and `Base.Index` conforms to `Hashable`.

- Equatable

  Conforms when `Base` conforms to `BidirectionalCollection` and `Base.Index` conforms to `Hashable`.

- Hashable

  Conforms when `Base` conforms to `BidirectionalCollection` and `Base.Index` conforms to `Hashable`.

- Sendable

  Conforms when `Base` conforms to `BidirectionalCollection` and `Base.Index` conforms to `Sendable`.

