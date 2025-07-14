

- SwiftData
-  HistoryTombstone 

Structure

# HistoryTombstone

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+Swift 5.9+

``` source
struct HistoryTombstone where Model : PersistentModel
```

## Topics

### Structures

struct Iterator

A type that provides the sequence’s iteration interface and encapsulates its iteration state.

### Instance Methods

func makeIterator() -> HistoryTombstone&lt;Model>.Iterator

Returns an iterator over the elements of this sequence.

### Subscripts

subscript(PartialKeyPath&lt;Model>) -> (any Sendable)?

### Type Aliases

typealias Element

A type representing the sequence’s elements.

### Default Implementations

Sequence Implementations

## Relationships

### Conforms To

- Sendable
- Sequence

