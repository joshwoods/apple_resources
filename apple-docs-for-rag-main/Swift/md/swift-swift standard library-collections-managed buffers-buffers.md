

- Swift
- Swift Standard Library
- Collections
-  Managed Buffers 

API Collection

# Managed Buffers

Build your own buffer-backed collection types.

## Topics

### Buffer Implementation

class ManagedBuffer

A class whose instances contain a property of type `Header` and raw storage for an array of `Element`, whose size is determined at instance creation.

struct ManagedBufferPointer

Contains a buffer object, and provides access to an instance of `Header` and contiguous storage for an arbitrary number of `Element` instances stored in that buffer.

### Uniqueness Checking

func isKnownUniquelyReferenced&lt;T>(inout T?) -> Bool

Returns a Boolean value indicating whether the given object is known to have a single strong reference.

func isKnownUniquelyReferenced&lt;T>(inout T) -> Bool

Returns a Boolean value indicating whether the given object is known to have a single strong reference.

## See Also

### Advanced Collection Topics

Sequence and Collection Protocols

Write generic code that works with any collection, or build your own collection types.

Supporting Types

Use wrappers, indices, and iterators in operations like slicing, flattening, and reversing a collection.

