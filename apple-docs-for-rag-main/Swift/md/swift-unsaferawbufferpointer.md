

- Swift
-  UnsafeRawBufferPointer 

Structure

# UnsafeRawBufferPointer

A nonowning collection interface to the bytes in a region of memory.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct UnsafeRawBufferPointer
```

## Overview

You can use an `UnsafeRawBufferPointer` instance in low-level operations to eliminate uniqueness checks and release mode bounds checks. Bounds checks are always performed in debug mode.

An `UnsafeRawBufferPointer` instance is a view of the raw bytes in a region of memory. Each byte in memory is viewed as a `UInt8` value independent of the type of values held in that memory. Reading from memory through a raw buffer is an untyped operation.

In addition to its collection interface, an `UnsafeRawBufferPointer` instance also supports the `load(fromByteOffset:as:)` and `loadUnaligned(fromByteOffset:as:)` methods provided by `UnsafeRawPointer`, including bounds checks in debug mode.

To access the underlying memory through typed operations, the memory must be bound to a trivial type.

Note

A *trivial type* can be copied bit for bit with no indirection or reference-counting operations. Generally, native Swift types that do not contain strong or weak references or other forms of indirection are trivial, as are imported C structs and enums. Copying memory that contains values of nontrivial types can only be done safely with a typed pointer. Copying bytes directly from nontrivial, in-memory values does not produce valid copies and can only be done by calling a C API, such as `memmove()`.

# UnsafeRawBufferPointer Semantics

An `UnsafeRawBufferPointer` instance is a view into memory and does not own the memory that it references. Copying a variable or constant of type `UnsafeRawBufferPointer` does not copy the underlying memory. However, initializing another collection with an `UnsafeRawBufferPointer` instance copies bytes out of the referenced memory and into the new collection.

The following example uses `someBytes`, an `UnsafeRawBufferPointer` instance, to demonstrate the difference between assigning a buffer pointer and using a buffer pointer as the source for another collection’s elements. Here, the assignment to `destBytes` creates a new, nonowning buffer pointer covering the first `n` bytes of the memory that `someBytes` references—nothing is copied:

```
var destBytes = someBytes[0..

Next, the bytes referenced by `destBytes` are copied into `byteArray`, a new `[UInt8]` array, and then the remainder of `someBytes` is appended to `byteArray`:

```
var byteArray: [UInt8] = Array(destBytes)
byteArray += someBytes[n..

## Topics

### Initializers

init(UnsafeRawBufferPointer)

Creates a new buffer over the same memory as the given buffer.

init(UnsafeMutableRawBufferPointer)

Creates a new buffer over the same memory as the given buffer.

init&lt;T>(UnsafeBufferPointer&lt;T>)

Creates a raw buffer over the contiguous bytes in the given typed buffer.

init&lt;T>(UnsafeMutableBufferPointer&lt;T>)

Creates a raw buffer over the contiguous bytes in the given typed buffer.

init(rebasing: Slice&lt;UnsafeRawBufferPointer>)

Creates a raw buffer over the same memory as the given raw buffer slice, with the indices rebased to zero.

init(rebasing: Slice&lt;UnsafeMutableRawBufferPointer>)

Creates a raw buffer over the same memory as the given raw buffer slice, with the indices rebased to zero.

init(start: UnsafeRawPointer?, count: Int)

Creates a buffer over the specified number of contiguous bytes starting at the given pointer.

### Instance Properties

var baseAddress: UnsafeRawPointer?

A pointer to the first byte of the buffer.

### Instance Methods

func assumingMemoryBound&lt;T>(to: T.Type) -> UnsafeBufferPointer&lt;T>

Returns a typed buffer to the memory referenced by this buffer, assuming that the memory is already bound to the specified type.

func bindMemory&lt;T>(to: T.Type) -> UnsafeBufferPointer&lt;T>

Binds this buffer’s memory to the specified type and returns a typed buffer of the bound memory.

func deallocate()

Deallocates the memory block previously allocated at this buffer pointer’s base address.

func load&lt;T>(fromByteOffset: Int, as: T.Type) -> T

Returns a new instance of the given type, read from the buffer pointer’s raw memory at the specified byte offset.

func loadUnaligned&lt;T>(fromByteOffset: Int, as: T.Type) -> T

Returns a new instance of the given type, constructed from the raw memory at the specified offset.

func loadUnaligned&lt;T>(fromByteOffset: Int, as: T.Type) -> T

func withMemoryRebound&lt;T, E, Result>(to: T.Type, (UnsafeBufferPointer&lt;T>) throws(E) -> Result) throws(E) -> Result

Executes the given closure while temporarily binding the buffer to instances of type `T`.

### Default Implementations

AtomicRepresentable Implementations

BidirectionalCollection Implementations

Collection Implementations

CustomDebugStringConvertible Implementations

RandomAccessCollection Implementations

Sequence Implementations

## Relationships

### Conforms To

- AtomicRepresentable
- BidirectionalCollection
- BitwiseCopyable
- Collection
- ContiguousBytes
- Copyable
- CustomDebugStringConvertible
- DataProtocol
- RandomAccessCollection
- Sequence

## See Also

### Raw Pointers

struct UnsafeRawPointer

A raw pointer for accessing untyped data.

struct UnsafeMutableRawPointer

A raw pointer for accessing and manipulating untyped data.

struct UnsafeMutableRawBufferPointer

A mutable nonowning collection interface to the bytes in a region of memory.

