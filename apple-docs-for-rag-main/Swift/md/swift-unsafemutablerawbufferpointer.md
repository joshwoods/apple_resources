

- Swift
-  UnsafeMutableRawBufferPointer 

Structure

# UnsafeMutableRawBufferPointer

A mutable nonowning collection interface to the bytes in a region of memory.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct UnsafeMutableRawBufferPointer
```

## Overview

You can use an `UnsafeMutableRawBufferPointer` instance in low-level operations to eliminate uniqueness checks and release mode bounds checks. Bounds checks are always performed in debug mode.

An `UnsafeMutableRawBufferPointer` instance is a view of the raw bytes in a region of memory. Each byte in memory is viewed as a `UInt8` value independent of the type of values held in that memory. Reading from and writing to memory through a raw buffer are untyped operations. Accessing this collection’s bytes does not bind the underlying memory to `UInt8`.

In addition to its collection interface, an `UnsafeMutableRawBufferPointer` instance also supports the following methods provided by `UnsafeMutableRawPointer`, including bounds checks in debug mode:

- `load(fromByteOffset:as:)`

- `loadUnaligned(fromByteOffset:as:)`

- `storeBytes(of:toByteOffset:as:)`

- `copyMemory(from:)`

To access the underlying memory through typed operations, the memory must be bound to a trivial type.

Note

A *trivial type* can be copied bit for bit with no indirection or reference-counting operations. Generally, native Swift types that do not contain strong or weak references or other forms of indirection are trivial, as are imported C structs and enums. Copying memory that contains values of nontrivial types can only be done safely with a typed pointer. Copying bytes directly from nontrivial, in-memory values does not produce valid copies and can only be done by calling a C API, such as `memmove()`.

# UnsafeMutableRawBufferPointer Semantics

An `UnsafeMutableRawBufferPointer` instance is a view into memory and does not own the memory that it references. Copying a variable or constant of type `UnsafeMutableRawBufferPointer` does not copy the underlying memory. However, initializing another collection with an `UnsafeMutableRawBufferPointer` instance copies bytes out of the referenced memory and into the new collection.

The following example uses `someBytes`, an `UnsafeMutableRawBufferPointer` instance, to demonstrate the difference between assigning a buffer pointer and using a buffer pointer as the source for another collection’s elements. Here, the assignment to `destBytes` creates a new, nonowning buffer pointer covering the first `n` bytes of the memory that `someBytes` references—nothing is copied:

```
var destBytes = someBytes[0..

Next, the bytes referenced by `destBytes` are copied into `byteArray`, a new `[UInt8]` array, and then the remainder of `someBytes` is appended to `byteArray`:

```
var byteArray: [UInt8] = Array(destBytes)
byteArray += someBytes[n..

Assigning into a ranged subscript of an `UnsafeMutableRawBufferPointer` instance copies bytes into the memory. The next `n` bytes of the memory that `someBytes` references are copied in this code:

```
destBytes[0..

## Topics

### Initializers

init(UnsafeMutableRawBufferPointer)

Creates a new buffer over the same memory as the given buffer.

init&lt;T>(UnsafeMutableBufferPointer&lt;T>)

Creates a raw buffer over the contiguous bytes in the given typed buffer.

init(mutating: UnsafeRawBufferPointer)

Creates a new mutable buffer over the same memory as the given buffer.

init(rebasing: Slice&lt;UnsafeMutableRawBufferPointer>)

Creates a raw buffer over the same memory as the given raw buffer slice, with the indices rebased to zero.

init(start: UnsafeMutableRawPointer?, count: Int)

Creates a buffer over the specified number of contiguous bytes starting at the given pointer.

### Instance Properties

var baseAddress: UnsafeMutableRawPointer?

A pointer to the first byte of the buffer.

### Instance Methods

func assumingMemoryBound&lt;T>(to: T.Type) -> UnsafeMutableBufferPointer&lt;T>

Returns a typed buffer to the memory referenced by this buffer, assuming that the memory is already bound to the specified type.

func bindMemory&lt;T>(to: T.Type) -> UnsafeMutableBufferPointer&lt;T>

Binds this buffer’s memory to the specified type and returns a typed buffer of the bound memory.

func copyBytes&lt;C>(from: C)

Copies from a collection of `UInt8` into this buffer’s memory.

func copyBytes(from: UnsafeRawBufferPointer)

func copyMemory(from: UnsafeRawBufferPointer)

Copies the bytes from the given buffer to this buffer’s memory.

func deallocate()

Deallocates the memory block previously allocated at this buffer pointer’s base address.

func initializeMemory&lt;S>(as: S.Element.Type, from: S) -> (unwritten: S.Iterator, initialized: UnsafeMutableBufferPointer&lt;S.Element>)

Initializes the buffer’s memory with the given elements, binding the initialized memory to the elements’ type.

func initializeMemory&lt;C>(as: C.Element.Type, fromContentsOf: C) -> UnsafeMutableBufferPointer&lt;C.Element>

Initializes the buffer’s memory with every element of the source, binding the initialized memory to the elements’ type.

func initializeMemory&lt;T>(as: T.Type, repeating: T) -> UnsafeMutableBufferPointer&lt;T>

Initializes the memory referenced by this buffer with the given value, binds the memory to the value’s type, and returns a typed buffer of the initialized memory.

func load&lt;T>(fromByteOffset: Int, as: T.Type) -> T

Returns a new instance of the given type, read from the buffer pointer’s raw memory at the specified byte offset.

func loadUnaligned&lt;T>(fromByteOffset: Int, as: T.Type) -> T

Returns a new instance of the given type, constructed from the raw memory at the specified offset.

func loadUnaligned&lt;T>(fromByteOffset: Int, as: T.Type) -> T

func moveInitializeMemory&lt;T>(as: T.Type, fromContentsOf: UnsafeMutableBufferPointer&lt;T>) -> UnsafeMutableBufferPointer&lt;T>

Moves every element of an initialized source buffer into the uninitialized memory referenced by this buffer, leaving the source memory uninitialized and this buffer’s memory initialized.

func moveInitializeMemory&lt;T>(as: T.Type, fromContentsOf: Slice&lt;UnsafeMutableBufferPointer&lt;T>>) -> UnsafeMutableBufferPointer&lt;T>

Moves every element of an initialized source buffer slice into the uninitialized memory referenced by this buffer, leaving the source memory uninitialized and this buffer’s memory initialized.

func storeBytes&lt;T>(of: T, toByteOffset: Int, as: T.Type)

Stores a value’s bytes into the buffer pointer’s raw memory at the specified byte offset.

func withMemoryRebound&lt;T, E, Result>(to: T.Type, (UnsafeMutableBufferPointer&lt;T>) throws(E) -> Result) throws(E) -> Result

Executes the given closure while temporarily binding the buffer to instances of type `T`.

### Type Methods

static func allocate(byteCount: Int, alignment: Int) -> UnsafeMutableRawBufferPointer

Allocates uninitialized memory with the specified size and alignment.

static func allocate(count: Int) -> UnsafeMutableRawBufferPointer

### Default Implementations

AtomicRepresentable Implementations

BidirectionalCollection Implementations

Collection Implementations

CustomDebugStringConvertible Implementations

MutableCollection Implementations

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
- MutableCollection
- RandomAccessCollection
- Sequence

## See Also

### Raw Pointers

struct UnsafeRawPointer

A raw pointer for accessing untyped data.

struct UnsafeMutableRawPointer

A raw pointer for accessing and manipulating untyped data.

struct UnsafeRawBufferPointer

A nonowning collection interface to the bytes in a region of memory.

