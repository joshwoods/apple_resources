

- Swift
- Array
- ArraySlice
-  RangeReplaceableCollection Implementations 

API Collection

# RangeReplaceableCollection Implementations

## Topics

### Operators

static func + &lt;Other>(Self, Other) -> Self

Creates a new collection by concatenating the elements of two collections.

static func + &lt;Other>(Other, Self) -> Self

Creates a new collection by concatenating the elements of a sequence and a collection.

static func + &lt;Other>(Self, Other) -> Self

Creates a new collection by concatenating the elements of a collection and a sequence.

static func += &lt;Other>(inout Self, Other)

Appends the elements of a sequence to a range-replaceable collection.

### Initializers

init()

Creates a new, empty array.

init&lt;S>(S)

Creates a new instance of a collection containing the elements of a sequence.

init(repeating: Element, count: Int)

Creates a new array containing the specified number of a single, repeated value.

init(repeating: Self.Element, count: Int)

Creates a new collection containing the specified number of a single, repeated value.

### Instance Methods

func append(Element)

Adds a new element at the end of the array.

func append(Self.Element)

Adds an element to the end of the collection.

func append&lt;S>(contentsOf: S)

Adds the elements of a sequence to the end of the array.

func append&lt;S>(contentsOf: S)

Adds the elements of a sequence or collection to the end of this collection.

func applying(CollectionDifference&lt;Self.Element>) -> Self?

Applies the given difference to this collection.

func insert(Self.Element, at: Self.Index)

Inserts a new element into the collection at the specified position.

func insert&lt;C>(contentsOf: C, at: Self.Index)

Inserts the elements of a sequence into the collection at the specified position.

func popLast() -> Self.Element?

Removes and returns the last element of the collection.

func popLast() -> Self.Element?

Removes and returns the last element of the collection.

func remove(at: Self.Index) -> Self.Element

Removes and returns the element at the specified position.

func removeAll(keepingCapacity: Bool)

Removes all elements from the array.

func removeAll(keepingCapacity: Bool)

Removes all elements from the collection.

func removeAll(where: (Self.Element) throws -> Bool) rethrows

Removes all the elements that satisfy the given predicate.

func removeAll(where: (Self.Element) throws -> Bool) rethrows

Removes all the elements that satisfy the given predicate.

func removeFirst() -> Self.Element

Removes and returns the first element of the collection.

func removeFirst() -> Self.Element

Removes and returns the first element of the collection.

func removeFirst(Int)

Removes the specified number of elements from the beginning of the collection.

func removeFirst(Int)

Removes the specified number of elements from the beginning of the collection.

func removeLast() -> Self.Element

Removes and returns the last element of the collection.

func removeLast() -> Self.Element

Removes and returns the last element of the collection.

func removeLast(Int)

Removes the specified number of elements from the end of the collection.

func removeLast(Int)

Removes the specified number of elements from the end of the collection.

func removeSubrange&lt;R>(R)

Removes the elements in the specified subrange from the collection.

func removeSubrange(Range&lt;Self.Index>)

Removes the elements in the specified subrange from the collection.

func removeSubranges(RangeSet&lt;Self.Index>)

Removes the elements at the given indices.

func replaceSubrange&lt;C>(Range&lt;Int>, with: C)

Replaces a range of elements with the elements in the specified collection.

func replaceSubrange&lt;C, R>(R, with: C)

Replaces the specified subrange of elements with the given collection.

func replaceSubrange&lt;C>(Range&lt;Self.Index>, with: C)

Replaces the specified subrange of elements with the given collection.

Deprecated

func reserveCapacity(Int)

Prepares the collection to store the specified number of elements, when doing so is appropriate for the underlying type.

