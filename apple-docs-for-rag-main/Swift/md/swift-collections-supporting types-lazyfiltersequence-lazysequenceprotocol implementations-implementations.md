

- Swift
- Swift Standard Library
- 
  - Swift Standard Library
- Collections
- Supporting Types
- LazyFilterSequence
-  LazySequenceProtocol Implementations 

API Collection

# LazySequenceProtocol Implementations

## Topics

### Instance Properties

var elements: Self

Identical to `self`.

var lazy: Self.Elements

### Instance Methods

func compactMap&lt;ElementOfResult>((Self.Elements.Element) -> ElementOfResult?) -> LazyMapSequence&lt;LazyFilterSequence&lt;LazyMapSequence&lt;Self.Elements, ElementOfResult?>>, ElementOfResult>

Returns the non-`nil` results of mapping the given transformation over this sequence.

func drop(while: (Self.Elements.Element) -> Bool) -> LazyDropWhileSequence&lt;Self.Elements>

Returns a lazy sequence that skips any initial elements that satisfy `predicate`.

func flatMap&lt;SegmentOfResult>((Self.Elements.Element) -> SegmentOfResult) -> LazySequence&lt;FlattenSequence&lt;LazyMapSequence&lt;Self.Elements, SegmentOfResult>>>

Returns the concatenated results of mapping the given transformation over this sequence.

func flatMap&lt;ElementOfResult>((Self.Elements.Element) -> ElementOfResult?) -> LazyMapSequence&lt;LazyFilterSequence&lt;LazyMapSequence&lt;Self.Elements, ElementOfResult?>>, ElementOfResult>

Returns the non-`nil` results of mapping the given transformation over this sequence.

func joined() -> LazySequence&lt;FlattenSequence&lt;Self.Elements>>

Returns a lazy sequence that concatenates the elements of this sequence of sequences.

func map&lt;U>((Self.Element) -> U) -> LazyMapSequence&lt;Self.Elements, U>

Returns a `LazyMapSequence` over this `Sequence`. The elements of the result are computed lazily, each time they are read, by calling `transform` function on a base element.

func prefix(while: (Self.Elements.Element) -> Bool) -> LazyPrefixWhileSequence&lt;Self.Elements>

Returns a lazy sequence of the initial consecutive elements that satisfy `predicate`.

### Type Aliases

typealias Elements

A `Sequence` that can contain the same elements as this one, possibly with a simpler type.

