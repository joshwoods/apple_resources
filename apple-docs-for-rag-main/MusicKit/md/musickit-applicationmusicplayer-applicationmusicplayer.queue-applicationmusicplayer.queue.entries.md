

- MusicKit
- ApplicationMusicPlayer
- ApplicationMusicPlayer.Queue
-  ApplicationMusicPlayer.Queue.Entries 

Structure

# ApplicationMusicPlayer.Queue.Entries

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 14.0+tvOS 15.0+visionOS 1.0+

``` source
struct Entries
```

## Topics

### Operators

static func == (ApplicationMusicPlayer.Queue.Entries, ApplicationMusicPlayer.Queue.Entries) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init()

Creates an empty collection of entries.

init(arrayLiteral: MusicPlayer.Queue.Entry...)

Creates an instance initialized with the given elements.

### Instance Properties

var endIndex: ApplicationMusicPlayer.Queue.Entries.Index

The collection’s “past the end” position—that is, the position one greater than the last valid subscript argument.

var hashValue: Int

The hash value.

var indices: ApplicationMusicPlayer.Queue.Entries.Indices

The indices that are valid for subscripting the collection, in ascending order.

var startIndex: ApplicationMusicPlayer.Queue.Entries.Index

The position of the first element in a nonempty collection.

### Instance Methods

func distance(from: ApplicationMusicPlayer.Queue.Entries.Index, to: ApplicationMusicPlayer.Queue.Entries.Index) -> Int

Returns the distance between two indices.

func formIndex(after: inout ApplicationMusicPlayer.Queue.Entries.Index)

Replaces the given index with its successor.

func formIndex(before: inout ApplicationMusicPlayer.Queue.Entries.Index)

Replaces the given index with its predecessor.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

func index(ApplicationMusicPlayer.Queue.Entries.Index, offsetBy: Int) -> ApplicationMusicPlayer.Queue.Entries.Index

Returns an index that is the specified distance from the given index.

func index(ApplicationMusicPlayer.Queue.Entries.Index, offsetBy: Int, limitedBy: ApplicationMusicPlayer.Queue.Entries.Index) -> ApplicationMusicPlayer.Queue.Entries.Index?

Returns an index that is the specified distance from the given index, unless that distance is beyond a given limiting index.

func index(after: ApplicationMusicPlayer.Queue.Entries.Index) -> ApplicationMusicPlayer.Queue.Entries.Index

Returns the position immediately after the given index.

func index(before: ApplicationMusicPlayer.Queue.Entries.Index) -> ApplicationMusicPlayer.Queue.Entries.Index

Returns the position immediately before the given index.

func makeIterator() -> ApplicationMusicPlayer.Queue.Entries.Iterator

Returns an iterator over the elements of this sequence.

func replaceSubrange&lt;C>(Range&lt;ApplicationMusicPlayer.Queue.Entries.Index>, with: C)

Replaces the specified subrange of elements with the given collection.

### Subscripts

subscript(Range&lt;ApplicationMusicPlayer.Queue.Entries.Index>) -> ApplicationMusicPlayer.Queue.Entries.SubSequence

Accesses a contiguous subrange of the collection’s elements.

subscript(ApplicationMusicPlayer.Queue.Entries.Index) -> ApplicationMusicPlayer.Queue.Entries.Element

Accesses the element at the specified position.

### Type Aliases

typealias ArrayLiteralElement

The type of the elements of an array literal.

typealias Element

A type representing the sequence’s elements.

typealias Index

A type that represents a position in the collection.

typealias Indices

A type that represents the indices that are valid for subscripting the collection, in ascending order.

typealias Iterator

A type that provides the sequence’s iteration interface and encapsulates its iteration state.

typealias SubSequence

A collection representing a contiguous subrange of this collection’s elements. The subsequence shares indices with the original collection.

### Default Implementations

BidirectionalCollection Implementations

Collection Implementations

Equatable Implementations

MutableCollection Implementations

RangeReplaceableCollection Implementations

Sequence Implementations

## Relationships

### Conforms To

- BidirectionalCollection
- Collection
- Equatable
- ExpressibleByArrayLiteral
- Hashable
- MutableCollection
- RandomAccessCollection
- RangeReplaceableCollection
- Sequence

