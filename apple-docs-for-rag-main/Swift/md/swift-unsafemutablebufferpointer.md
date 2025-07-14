

- Swift
-  UnsafeMutableBufferPointer 

Structure

# UnsafeMutableBufferPointer

A nonowning collection interface to a buffer of mutable elements stored contiguously in memory.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct UnsafeMutableBufferPointer where Element : ~Copyable
```

## Overview

You can use an `UnsafeMutableBufferPointer` instance in low level operations to eliminate uniqueness checks and, in release mode, bounds checks. Bounds checks are always performed in debug mode.

# UnsafeMutableBufferPointer Semantics

An `UnsafeMutableBufferPointer` instance is a view into memory and does not own the memory that it references. Copying a value of type `UnsafeMutableBufferPointer` does not copy the instances stored in the underlying memory. However, initializing another collection with an `UnsafeMutableBufferPointer` instance copies the instances out of the referenced memory and into the new collection.

## Topics

### Initializers

init(AudioBuffer)

Initialize an `UnsafeMutableBufferPointer` from an `AudioBuffer`.

init(MLMultiArray) throws

init(mutating: UnsafeBufferPointer&lt;Element>)

Creates a mutable typed buffer pointer referencing the same memory as the given immutable buffer pointer.

init(rebasing: Slice&lt;UnsafeMutableBufferPointer&lt;Element>>)

Creates a buffer over the same memory as the given buffer slice.

init(start: UnsafeMutablePointer&lt;Element>?, count: Int)

Creates a new buffer pointer over the specified number of contiguous instances beginning at the given pointer.

### Instance Properties

var baseAddress: UnsafeMutablePointer&lt;Element>?

A pointer to the first element of the buffer.

let count: Int

The number of elements in the buffer.

### Instance Methods

func assign(repeating: Element)Deprecated

func deallocate()

Deallocates the memory block previously allocated at this buffer pointer’s base address.

func deinitialize() -> UnsafeMutableRawBufferPointer

Deinitializes every instance in this buffer.

func deinitializeElement(at: UnsafeMutableBufferPointer&lt;Element>.Index)

Deinitializes the memory underlying the element at `index`.

func extracting(Range&lt;Int>) -> UnsafeMutableBufferPointer&lt;Element>

Constructs a standalone buffer pointer over the items within the supplied range of positions in the memory region addressed by this buffer pointer.

func extracting(some RangeExpression&lt;Int>) -> UnsafeMutableBufferPointer&lt;Element>

Constructs a standalone buffer pointer over the items within the supplied range of positions in the memory region addressed by this buffer pointer.

func extracting((UnboundedRange_) -> ()) -> UnsafeMutableBufferPointer&lt;Element>

Extracts and returns a copy of the entire buffer.

func initialize&lt;S>(from: S) -> (unwritten: S.Iterator, index: UnsafeMutableBufferPointer&lt;Element>.Index)

Initializes the buffer’s memory with the given elements.

func initialize(fromContentsOf: some Collection&lt;Element>) -> UnsafeMutableBufferPointer&lt;Element>.Index

Initializes the buffer’s memory with every element of the source.

func initialize(repeating: Element)

Initializes every element in this buffer’s memory to a copy of the given value.

func initializeElement(at: UnsafeMutableBufferPointer&lt;Element>.Index, to: consuming Element)

Initializes the element at `index` to the given value.

func moveElement(from: UnsafeMutableBufferPointer&lt;Element>.Index) -> Element

Retrieves and returns the element at `index`, leaving that element’s underlying memory uninitialized.

func moveInitialize(fromContentsOf: Slice&lt;UnsafeMutableBufferPointer&lt;Element>>) -> UnsafeMutableBufferPointer&lt;Element>.Index

Moves every element of an initialized source buffer into the uninitialized memory referenced by this buffer, leaving the source memory uninitialized and this buffer’s memory initialized.

func moveInitialize(fromContentsOf: UnsafeMutableBufferPointer&lt;Element>) -> UnsafeMutableBufferPointer&lt;Element>.Index

Moves every element of an initialized source buffer into the uninitialized memory referenced by this buffer, leaving the source memory uninitialized and this buffer’s memory initialized.

func moveUpdate(fromContentsOf: Slice&lt;UnsafeMutableBufferPointer&lt;Element>>) -> UnsafeMutableBufferPointer&lt;Element>.Index

Updates this buffer’s initialized memory initialized memory by moving every element from the source buffer slice, leaving the source memory uninitialized.

func moveUpdate(fromContentsOf: UnsafeMutableBufferPointer&lt;Element>) -> UnsafeMutableBufferPointer&lt;Element>.Index

Updates this buffer’s initialized memory initialized memory by moving every element from the source buffer, leaving the source memory uninitialized.

func update&lt;S>(from: S) -> (unwritten: S.Iterator, index: UnsafeMutableBufferPointer&lt;Element>.Index)

Updates the buffer’s initialized memory with the given elements.

func update(fromContentsOf: some Collection&lt;Element>) -> UnsafeMutableBufferPointer&lt;Element>.Index

Updates the buffer’s initialized memory with every element of the source.

func update(repeating: Element)

Updates every element of this buffer’s initialized memory.

func withMemoryRebound&lt;T, E, Result>(to: T.Type, (UnsafeMutableBufferPointer&lt;T>) throws(E) -> Result) throws(E) -> Result

Executes the given closure while temporarily binding the memory referenced by this buffer to the given type.

### Subscripts

subscript(Int) -> Element

Accesses the element at the specified position.

### Type Methods

static func allocate(capacity: Int) -> UnsafeMutableBufferPointer&lt;Element>

Allocates uninitialized memory for the specified number of instances of type `Element`.

### Default Implementations

AtomicRepresentable Implementations

BidirectionalCollection Implementations

Collection Implementations

CustomDebugStringConvertible Implementations

MutableCollection Implementations

Sequence Implementations

## Relationships

### Conforms To

- AccelerateBuffer
- AccelerateMutableBuffer
- AtomicRepresentable

  Conforms when `Element` conforms to `Escapable`.

- BNNSGraph.PointerArgument
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

- MutableCollection

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

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

struct UnsafeBufferPointer

A nonowning collection interface to a buffer of elements stored contiguously in memory.

