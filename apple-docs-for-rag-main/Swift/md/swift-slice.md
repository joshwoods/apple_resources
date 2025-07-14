

- Swift
-  Slice 

Structure

# Slice

A view into a subsequence of elements of another collection.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct Slice where Base : Collection
```

## Overview

A slice stores a base collection and the start and end indices of the view. It does not copy the elements from the collection into separate storage. Thus, creating a slice has O(1) complexity.

## Slices Share Indices

Indices of a slice can be used interchangeably with indices of the base collection. An element of a slice is located under the same index in the slice and in the base collection, as long as neither the collection nor the slice has been mutated since the slice was created.

For example, suppose you have an array holding the number of absences from each class during a session.

```
var absences = [0, 2, 0, 4, 0, 3, 1, 0]
```

You’re tasked with finding the day with the most absences in the second half of the session. To find the index of the day in question, follow these steps:

1.  Create a slice of the `absences` array that holds the second half of the days.

2.  Use the `max(by:)` method to determine the index of the day with the most absences.

3.  Print the result using the index found in step 2 on the original `absences` array.

Here’s an implementation of those steps:

```
let secondHalf = absences.suffix(absences.count / 2)
if let i = secondHalf.indices.max(by: { secondHalf[$0] 

## Slices Inherit Semantics

A slice inherits the value or reference semantics of its base collection. That is, if a `Slice` instance is wrapped around a mutable collection that has value semantics, such as an array, mutating the original collection would trigger a copy of that collection, and not affect the base collection stored inside of the slice.

For example, if you update the last element of the `absences` array from `0` to `2`, the `secondHalf` slice is unchanged.

```
absences[7] = 2
print(absences)
// Prints "[0, 2, 0, 4, 0, 3, 1, 2]"
print(secondHalf)
// Prints "[0, 3, 1, 0]"
```

Use slices only for transient computation. A slice may hold a reference to the entire storage of a larger collection, not just to the portion it presents, even after the base collection’s lifetime ends. Long-term storage of a slice may therefore prolong the lifetime of elements that are no longer otherwise accessible, which can erroneously appear to be memory leakage.

Note

Using a `Slice` instance with a mutable collection requires that the base collection’s `subscript(_: Index)` setter does not invalidate indices. If mutations need to invalidate indices in your custom collection type, don’t use `Slice` as its subsequence type. Instead, define your own subsequence type that takes your index invalidation requirements into account.

## Topics

### Initializers

init(base: Base, bounds: Range&lt;Base.Index>)

Creates a view into the given collection that allows access to elements within the specified range.

### Instance Properties

var base: Base

The underlying collection of the slice.

### Instance Methods

func assumingMemoryBound&lt;T>(to: T.Type) -> UnsafeMutableBufferPointer&lt;T>

Returns a typed buffer to the memory referenced by this buffer slice, assuming that the memory is already bound to the specified type.

func assumingMemoryBound&lt;T>(to: T.Type) -> UnsafeBufferPointer&lt;T>

Returns a typed buffer to the memory referenced by this buffer slice, assuming that the memory is already bound to the specified type.

func bindMemory&lt;T>(to: T.Type) -> UnsafeMutableBufferPointer&lt;T>

Binds this buffer slice’s memory to the specified type and returns a typed buffer of the bound memory.

func bindMemory&lt;T>(to: T.Type) -> UnsafeBufferPointer&lt;T>

Binds this buffer slice’s memory to the specified type and returns a typed buffer of the bound memory.

func copyBytes&lt;C>(from: C)

Copies from a collection of `UInt8` into this buffer slice’s memory.

func deinitialize&lt;Element>() -> UnsafeMutableRawBufferPointer

Deinitializes every instance in this buffer slice.

func deinitializeElement&lt;Element>(at: UnsafeMutableBufferPointer&lt;Element>.Index)

Deinitializes the memory underlying the element at `index`.

func initialize&lt;S>(from: S) -> (unwritten: S.Iterator, index: Slice&lt;Base>.Index)

Initializes the buffer slice’s memory with the given elements.

func initialize&lt;Element>(fromContentsOf: some Collection) -> Slice&lt;Base>.Index

Initializes the buffer slice’s memory with with every element of the source.

func initialize&lt;Element>(repeating: Element)

Initializes every element in this buffer slice’s memory to a copy of the given value.

func initializeElement&lt;Element>(at: Int, to: Element)

Initializes the element at `index` to the given value.

func initializeMemory&lt;S>(as: S.Element.Type, from: S) -> (unwritten: S.Iterator, initialized: UnsafeMutableBufferPointer&lt;S.Element>)

Initializes the buffer’s memory with the given elements, binding the initialized memory to the elements’ type.

func initializeMemory&lt;C>(as: C.Element.Type, fromContentsOf: C) -> UnsafeMutableBufferPointer&lt;C.Element>

Initializes the buffer slice’s memory with every element of the source, binding the initialized memory to the elements’ type.

func initializeMemory&lt;T>(as: T.Type, repeating: T) -> UnsafeMutableBufferPointer&lt;T>

Initializes the memory referenced by this buffer slice with the given value, binds the memory to the value’s type, and returns a typed buffer of the initialized memory.

func insert(Base.Element, at: Slice&lt;Base>.Index)

func insert&lt;S>(contentsOf: S, at: Slice&lt;Base>.Index)

func load&lt;T>(fromByteOffset: Int, as: T.Type) -> T

Returns a new instance of the given type, read from the specified offset into the buffer pointer slice’s raw memory.

func load&lt;T>(fromByteOffset: Int, as: T.Type) -> T

Returns a new instance of the given type, read from the specified offset into the buffer pointer slice’s raw memory.

func loadUnaligned&lt;T>(fromByteOffset: Int, as: T.Type) -> T

func loadUnaligned&lt;T>(fromByteOffset: Int, as: T.Type) -> T

Returns a new instance of the given type, read from the specified offset into the buffer pointer slice’s raw memory.

func loadUnaligned&lt;T>(fromByteOffset: Int, as: T.Type) -> T

Returns a new instance of the given type, read from the specified offset into the buffer pointer slice’s raw memory.

func loadUnaligned&lt;T>(fromByteOffset: Int, as: T.Type) -> T

func moveElement&lt;Element>(from: Slice&lt;Base>.Index) -> Element

Retrieves and returns the element at `index`, leaving that element’s underlying memory uninitialized.

func moveInitialize&lt;Element>(fromContentsOf: UnsafeMutableBufferPointer&lt;Element>) -> Slice&lt;Base>.Index

Moves every element of an initialized source buffer into the uninitialized memory referenced by this buffer slice, leaving the source memory uninitialized and this buffer slice’s memory initialized.

func moveInitialize&lt;Element>(fromContentsOf: Slice&lt;UnsafeMutableBufferPointer&lt;Element>>) -> Slice&lt;Base>.Index

Moves every element of an initialized source buffer slice into the uninitialized memory referenced by this buffer slice, leaving the source memory uninitialized and this buffer slice’s memory initialized.

func moveInitializeMemory&lt;T>(as: T.Type, fromContentsOf: Slice&lt;UnsafeMutableBufferPointer&lt;T>>) -> UnsafeMutableBufferPointer&lt;T>

Moves every element from an initialized source buffer slice into the uninitialized memory referenced by this buffer slice, leaving the source memory uninitialized and this slice’s memory initialized.

func moveInitializeMemory&lt;T>(as: T.Type, fromContentsOf: UnsafeMutableBufferPointer&lt;T>) -> UnsafeMutableBufferPointer&lt;T>

Moves every element of an initialized source buffer into the uninitialized memory referenced by this buffer slice, leaving the source memory uninitialized and this slice’s memory initialized.

func moveUpdate&lt;Element>(fromContentsOf: UnsafeMutableBufferPointer&lt;Element>) -> Slice&lt;Base>.Index

Updates this buffer slice’s initialized memory initialized memory by moving every element from the source buffer, leaving the source memory uninitialized.

func moveUpdate&lt;Element>(fromContentsOf: Slice&lt;UnsafeMutableBufferPointer&lt;Element>>) -> Slice&lt;Base>.Index

Updates this buffer slice’s initialized memory initialized memory by moving every element from the source buffer slice, leaving the source memory uninitialized.

func remove(at: Slice&lt;Base>.Index) -> Base.Element

func removeSubrange(Range&lt;Slice&lt;Base>.Index>)

func replaceSubrange&lt;C>(Range&lt;Slice&lt;Base>.Index>, with: C)

func storeBytes&lt;T>(of: T, toByteOffset: Int, as: T.Type)

Stores a value’s bytes into the buffer pointer slice’s raw memory at the specified byte offset.

func update&lt;S>(from: S) -> (unwritten: S.Iterator, index: Slice&lt;Base>.Index)

Updates the buffer slice’s initialized memory with the given elements.

func update&lt;Element>(fromContentsOf: some Collection) -> Slice&lt;Base>.Index

Updates the buffer slice’s initialized memory with every element of the source.

func update&lt;Element>(repeating: Element)

Updates every element of this buffer slice’s initialized memory.

func withContiguousMutableStorageIfAvailable&lt;R, Element>((inout UnsafeMutableBufferPointer&lt;Element>) throws -> R) rethrows -> R?

func withMemoryRebound&lt;T, Result, Element>(to: T.Type, (UnsafeMutableBufferPointer&lt;T>) throws -> Result) rethrows -> Result

Executes the given closure while temporarily binding the memory referenced by this buffer slice to the given type.

func withMemoryRebound&lt;T, Result, E>(to: T.Type, (UnsafeBufferPointer&lt;T>) throws(E) -> Result) throws(E) -> Result

Executes the given closure while temporarily binding the buffer slice to instances of type `T`.

func withMemoryRebound&lt;T, Result, E>(to: T.Type, (UnsafeMutableBufferPointer&lt;T>) throws(E) -> Result) throws(E) -> Result

Executes the given closure while temporarily binding the buffer slice to instances of type `T`.

func withMemoryRebound&lt;T, Result, Element>(to: T.Type, (UnsafeBufferPointer&lt;T>) throws -> Result) rethrows -> Result

Executes the given closure while temporarily binding the memory referenced by this buffer slice to the given type.

### Default Implementations

BidirectionalCollection Implementations

Collection Implementations

LazySequenceProtocol Implementations

MutableCollection Implementations

RangeReplaceableCollection Implementations

Sequence Implementations

## Relationships

### Conforms To

- AccelerateBuffer
- AccelerateMutableBuffer
- BidirectionalCollection

  Conforms when `Base` conforms to `BidirectionalCollection`.

- Collection

  Conforms when `Base` conforms to `BidirectionalCollection`.

- ContiguousBytes
- Copyable

  Conforms when `Base` conforms to `Collection`.

- DataProtocol
- LazySequenceProtocol

  Conforms when `Base` conforms to `Collection` and `LazySequenceProtocol`.

- MutableCollection

  Conforms when `Base` conforms to `MutableCollection`.

- RandomAccessCollection

  Conforms when `Base` conforms to `RandomAccessCollection`.

- RangeReplaceableCollection

  Conforms when `Base` conforms to `RangeReplaceableCollection`.

- Sendable

  Conforms when `Base` conforms to `Collection`, `Base` conforms to `Sendable`, and `Base.Index` conforms to `Sendable`.

- Sequence

  Conforms when `Base` conforms to `Collection` and `LazySequenceProtocol`.

