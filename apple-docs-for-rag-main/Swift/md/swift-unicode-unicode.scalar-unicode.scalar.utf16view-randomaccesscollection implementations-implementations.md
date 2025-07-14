

- Swift
- Swift Standard Library
- Strings and Text
- 
  - Swift Standard Library
  - Strings and Text
- Unicode
- Unicode.Scalar
- Unicode.Scalar.UTF16View
-  RandomAccessCollection Implementations 

API Collection

# RandomAccessCollection Implementations

## Topics

### Instance Properties

var endIndex: Int

The “past the end” position—that is, the position one greater than the last valid subscript argument.

var startIndex: Int

The position of the first code unit.

### Instance Methods

func index(Self.Index, offsetBy: Int, limitedBy: Self.Index) -> Self.Index?

Returns an index that is the specified distance from the given index, unless that distance is beyond a given limiting index.

### Subscripts

subscript(Int) -> UTF16.CodeUnit

Accesses the code unit at the specified position.

