

- Swift
- Swift Standard Library
- Collections
- KeyValuePairs
-  RandomAccessCollection Implementations 

API Collection

# RandomAccessCollection Implementations

## Topics

### Instance Properties

var endIndex: KeyValuePairs&lt;Key, Value>.Index

The collection’s “past the end” position—that is, the position one greater than the last valid subscript argument.

var startIndex: KeyValuePairs&lt;Key, Value>.Index

The position of the first element in a nonempty collection.

### Instance Methods

func index(Self.Index, offsetBy: Int, limitedBy: Self.Index) -> Self.Index?

Returns an index that is the specified distance from the given index, unless that distance is beyond a given limiting index.

### Subscripts

subscript(KeyValuePairs&lt;Key, Value>.Index) -> KeyValuePairs&lt;Key, Value>.Element

Accesses the element at the specified position.

### Type Aliases

typealias Element

The element type of a `KeyValuePairs`: a tuple containing an individual key-value pair.

