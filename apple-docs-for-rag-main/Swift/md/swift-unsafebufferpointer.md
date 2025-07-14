

- Swift
-  UnsafeBufferPointer 

Structure

# UnsafeBufferPointer

A nonowning collection interface to a buffer of elements stored contiguously in memory.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct UnsafeBufferPointer where Element : ~Copyable
```

## Overview

You can use an `UnsafeBufferPointer` instance in low level operations to eliminate uniqueness checks and, in release mode, bounds checks. Bounds checks are always performed in debug mode.

# UnsafeBufferPointer Semantics

An `UnsafeBufferPointer` instance is a view into memory and does not own the memory that it references. Copying a value of type `UnsafeBufferPointer` does not copy the instances stored in the underlying memory. However, initializing another collection with an `UnsafeBufferPointer` instance copies the instances out of the referenced memory and into the new collection.

## Topics

### Initializers

init(MLMultiArray) throws

init(UnsafeMutableBufferPointer&lt;Element>)

Creates an immutable typed buffer pointer referencing the same memory as the given mutable buffer pointer.

init(AudioBuffer)

Initialize an `UnsafeBufferPointer` from an `AudioBuffer`. Binds the buffer’s memory type to `Element`.

init(rebasing: Slice&lt;UnsafeMutableBufferPointer&lt;Element>>)

Creates a buffer over the same memory as the given buffer slice.

init(rebasing: Slice&lt;UnsafeBufferPointer&lt;Element>>)

Creates a buffer over the same memory as the given buffer slice.

init(start: UnsafePointer&lt;Element>?, count: Int)

Creates a new buffer pointer over the specified number of contiguous instances beginning at the given pointer.

### Instance Properties

var baseAddress: UnsafePointer&lt;Element>?

A pointer to the first element of the buffer.

let count: Int

The number of elements in the buffer.

### Instance Methods

func deallocate()

Deallocates the memory block previously allocated at this buffer pointer’s base address.

func extracting(some RangeExpression&lt;Int>) -> UnsafeBufferPointer&lt;Element>

Constructs a standalone buffer pointer over the items within the supplied range of positions in the memory region addressed by this buffer pointer.

func extracting((UnboundedRange_) -> ()) -> UnsafeBufferPointer&lt;Element>

Extracts and returns a copy of the entire buffer.

func extracting(Range&lt;Int>) -> UnsafeBufferPointer&lt;Element>

Constructs a standalone buffer pointer over the items within the supplied range of positions in the memory region addressed by this buffer pointer.

func withMemoryRebound&lt;T, E, Result>(to: T.Type, (UnsafeBufferPointer&lt;T>) throws(E) -> Result) throws(E) -> Result

Executes the given closure while temporarily binding the memory referenced by this buffer to the given type.

### Subscripts

subscript(Int) -> Element

Accesses the element at the specified position.

### Default Implementations

AtomicRepresentable Implementations

BidirectionalCollection Implementations

Collection Implementations

CustomDebugStringConvertible Implementations

Sequence Implementations

## Relationships

### Conforms To

- AccelerateBuffer
- AtomicRepresentable

  Conforms when `Element` conforms to `Escapable`.

- BidirectionalCollection

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- BitwiseCopyable

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- Collection

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- ContiguousBytes
- Copyable

  Conforms when `Element` conforms to `Escapable`.

- CustomDebugStringConvertible

  Conforms when `Element` conforms to `Escapable`.

- DataProtocol
- RandomAccessCollection

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- Sequence

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

## See Also

### Typed Pointers

struct UnsafePointer

A pointer for accessing data of a specific type.

struct UnsafeMutablePointer

A pointer for accessing and manipulating data of a specific type.

struct UnsafeMutableBufferPointer

A nonowning collection interface to a buffer of mutable elements stored contiguously in memory.

