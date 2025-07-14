

- Swift
- Swift Standard Library
- 
  - Swift Standard Library
- Collections
- Supporting Types
- Repeated
-  RandomAccessCollection Implementations 

API Collection

# RandomAccessCollection Implementations

## Topics

### Instance Properties

var endIndex: Repeated&lt;Element>.Index

The collection’s “past the end” position—that is, the position one greater than the last valid subscript argument.

var startIndex: Repeated&lt;Element>.Index

The position of the first element in a nonempty collection.

### Instance Methods

func index(Self.Index, offsetBy: Int, limitedBy: Self.Index) -> Self.Index?

Returns an index that is the specified distance from the given index, unless that distance is beyond a given limiting index.

### Subscripts

subscript(Int) -> Element

Accesses the element at the specified position.

### Type Aliases

typealias Index

A type that represents a valid position in the collection.

