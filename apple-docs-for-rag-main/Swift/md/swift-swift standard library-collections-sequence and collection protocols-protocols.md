

- Swift
- Swift Standard Library
- Collections
-  Sequence and Collection Protocols 

API Collection

# Sequence and Collection Protocols

Write generic code that works with any collection, or build your own collection types.

## Topics

### First Steps

protocol Sequence

A type that provides sequential, iterated access to its elements.

protocol Collection

A sequence whose elements can be traversed multiple times, nondestructively, and accessed by an indexed subscript.

### Collection Traversal

protocol BidirectionalCollection

A collection that supports backward as well as forward traversal.

protocol RandomAccessCollection

A collection that supports efficient random-access index traversal.

### Collection Mutability

protocol MutableCollection

A collection that supports subscript assignment.

protocol RangeReplaceableCollection

A collection that supports replacement of an arbitrary subrange of elements with the elements of another collection.

### Manual Iteration

protocol IteratorProtocol

A type that supplies the values of a sequence one at a time.

### Algebraic Sets

protocol SetAlgebra

A type that provides mathematical set operations.

### Lazy Collections

protocol LazySequenceProtocol

A sequence on which normally-eager sequence operations are implemented lazily.

protocol LazyCollectionProtocol

## See Also

### Advanced Collection Topics

Supporting Types

Use wrappers, indices, and iterators in operations like slicing, flattening, and reversing a collection.

Managed Buffers

Build your own buffer-backed collection types.

