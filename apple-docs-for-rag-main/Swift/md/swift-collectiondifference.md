

- Swift
-  CollectionDifference 

Structure

# CollectionDifference

A collection of insertions and removals that describe the difference between two ordered collection states.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct CollectionDifference
```

## Topics

### Initializers

init?&lt;Changes>(Changes)

Creates a new collection difference from a collection of changes.

### Instance Properties

let insertions: [CollectionDifference&lt;ChangeElement>.Change]

The insertions contained by this difference, from lowest offset to highest.

let removals: [CollectionDifference&lt;ChangeElement>.Change]

The removals contained by this difference, from lowest offset to highest.

### Instance Methods

func formIndex(inout CollectionDifference&lt;ChangeElement>.Index, offsetBy: Int)

func index(before: CollectionDifference&lt;ChangeElement>.Index) -> CollectionDifference&lt;ChangeElement>.Index

func inferringMoves() -> CollectionDifference&lt;ChangeElement>

Returns a new collection difference with associations between individual elements that have been removed and inserted only once.

func inverse() -> CollectionDifference&lt;ChangeElement>

### Enumerations

enum Change

A single change to a collection.

### Default Implementations

Collection Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

Hashable Implementations

Sequence Implementations

## Relationships

### Conforms To

- Collection

  Conforms when `ChangeElement` conforms to `Copyable` and `Escapable`.

- Copyable

  Conforms when `ChangeElement` conforms to `Equatable`.

- Decodable

  Conforms when `ChangeElement` conforms to `Decodable` and `Encodable`.

- Encodable

  Conforms when `ChangeElement` conforms to `Decodable` and `Encodable`.

- Equatable

  Conforms when `ChangeElement` conforms to `Equatable`.

- Hashable

  Conforms when `ChangeElement` conforms to `Hashable`.

- Sendable

  Conforms when `ChangeElement` conforms to `Copyable`, `Escapable`, and `Sendable`.

- Sequence

  Conforms when `ChangeElement` conforms to `Copyable` and `Escapable`.

## See Also

### Wrappers for Algorithms

struct DropFirstSequence

A sequence that lazily consumes and drops `n` elements from an underlying `Base` iterator before possibly returning the first available element.

struct DropWhileSequence

A sequence that lazily consumes and drops `n` elements from an underlying `Base` iterator before possibly returning the first available element.

struct EnumeratedSequence

An enumeration of the elements of a sequence or collection.

typealias FlattenCollection

struct FlattenSequence

A sequence consisting of all the elements contained in each segment contained in some `Base` sequence.

struct JoinedSequence

A sequence that presents the elements of a base sequence of sequences concatenated using a given separator.

struct PrefixSequence

A sequence that only consumes up to `n` elements from an underlying `Base` iterator.

struct Repeated

A collection whose elements are all identical.

struct ReversedCollection

A collection that presents the elements of its base collection in reverse order.

struct StrideTo

A sequence of values formed by striding over a half-open interval.

struct StrideThrough

A sequence of values formed by striding over a closed interval.

struct UnfoldSequence

A sequence whose elements are produced via repeated applications of a closure to some mutable state.

struct Zip2Sequence

A sequence of pairs built out of two underlying sequences.

