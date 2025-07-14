

- Swift
-  DiscontiguousSlice 

Structure

# DiscontiguousSlice

A collection wrapper that provides access to the elements of a collection, indexed by a set of indices.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct DiscontiguousSlice where Base : Collection
```

## Topics

### Instance Properties

var base: Base

The collection that the indexed collection wraps.

let subranges: RangeSet&lt;Base.Index>

The set of subranges that are available through this discontiguous slice.

### Subscripts

subscript(DiscontiguousSlice&lt;Base>.Index) -> Base.Element

Accesses the element at the specified position.

### Default Implementations

BidirectionalCollection Implementations

Collection Implementations

CustomStringConvertible Implementations

Equatable Implementations

Hashable Implementations

Sequence Implementations

## Relationships

### Conforms To

- BidirectionalCollection

  Conforms when `Base` conforms to `BidirectionalCollection`.

- Collection

  Conforms when `Base` conforms to `BidirectionalCollection`.

- Copyable

  Conforms when `Base` conforms to `Collection` and `Base.Element` conforms to `Hashable`.

- CustomStringConvertible

  Conforms when `Base` conforms to `Collection`.

- Equatable

  Conforms when `Base` conforms to `Collection` and `Base.Element` conforms to `Hashable`.

- Hashable

  Conforms when `Base` conforms to `Collection` and `Base.Element` conforms to `Hashable`.

- Sendable

  Conforms when `Base` conforms to `Collection`, `Base` conforms to `Sendable`, and `Base.Index` conforms to `Sendable`.

- Sequence

  Conforms when `Base` conforms to `Collection`.

