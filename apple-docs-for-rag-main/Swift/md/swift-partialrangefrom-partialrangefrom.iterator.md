

- Swift
- PartialRangeFrom
-  PartialRangeFrom.Iterator 

Structure

# PartialRangeFrom.Iterator

The iterator for a `PartialRangeFrom` instance.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct Iterator
```

Available when `Bound` conforms to `Strideable` and `Bound.Stride` conforms to `SignedInteger`.

## Topics

### Instance Methods

func next() -> Bound?

Advances to the next element and returns it, or `nil` if no next element exists.

### Type Aliases

typealias Element

The type of element traversed by the iterator.

## Relationships

### Conforms To

- IteratorProtocol
- Sendable

  Conforms when `Bound` conforms to `Sendable`, `Bound` conforms to `Strideable`, and `Bound.Stride` conforms to `SignedInteger`.

