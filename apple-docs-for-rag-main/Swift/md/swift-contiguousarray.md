

- Swift
-  ContiguousArray 

Structure

# ContiguousArray

A contiguously stored array.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct ContiguousArray
```

## Overview

The `ContiguousArray` type is a specialized array that always stores its elements in a contiguous region of memory. This contrasts with `Array`, which can store its elements in either a contiguous region of memory or an `NSArray` instance if its `Element` type is a class or `@objc` protocol.

If your array’s `Element` type is a class or `@objc` protocol and you do not need to bridge the array to `NSArray` or pass the array to Objective-C APIs, using `ContiguousArray` may be more efficient and have more predictable performance than `Array`. If the array’s `Element` type is a struct or enumeration, `Array` and `ContiguousArray` should have similar efficiency.

For more information about using arrays, see `Array` and `ArraySlice`, with which `ContiguousArray` shares most properties and methods.

## Topics

### Initializers

init&lt;S>(S)

Creates an array containing the elements of a sequence.

init(unsafeUninitializedCapacity: Int, initializingWith: (inout UnsafeMutableBufferPointer&lt;Element>, inout Int) throws -> Void) rethrows

Creates an array with the specified capacity, then calls the given closure with a buffer covering the array’s uninitialized memory.

### Instance Properties

var capacity: Int

The total number of elements that the array can contain without allocating new storage.

### Instance Methods

func insert(Element, at: Int)

Inserts a new element at the specified position.

func remove(at: Int) -> Element

Removes and returns the element at the specified position.

func reserveCapacity(Int)

Reserves enough space to store the specified number of elements.

func withUnsafeBufferPointer&lt;R, E>((UnsafeBufferPointer&lt;Element>) throws(E) -> R) throws(E) -> R

Calls a closure with a pointer to the array’s contiguous storage.

func withUnsafeBytes&lt;R>((UnsafeRawBufferPointer) throws -> R) rethrows -> R

Calls the given closure with a pointer to the underlying bytes of the array’s contiguous storage.

func withUnsafeMutableBufferPointer&lt;R, E>((inout UnsafeMutableBufferPointer&lt;Element>) throws(E) -> R) throws(E) -> R

Calls the given closure with a pointer to the array’s mutable contiguous storage.

func withUnsafeMutableBytes&lt;R>((UnsafeMutableRawBufferPointer) throws -> R) rethrows -> R

Calls the given closure with a pointer to the underlying bytes of the array’s mutable contiguous storage.

### Default Implementations

BidirectionalCollection Implementations

Collection Implementations

CustomDebugStringConvertible Implementations

CustomReflectable Implementations

CustomStringConvertible Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

ExpressibleByArrayLiteral Implementations

Hashable Implementations

MutableCollection Implementations

RandomAccessCollection Implementations

RangeReplaceableCollection Implementations

Sequence Implementations

## Relationships

### Conforms To

- AccelerateBuffer
- AccelerateMutableBuffer
- BidirectionalCollection

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- Collection

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- ContiguousBytes
- Copyable

  Conforms when `Element` conforms to `Hashable`.

- CustomDebugStringConvertible

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- CustomReflectable

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- CustomStringConvertible

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- DataProtocol
- Decodable

  Conforms when `Element` conforms to `Decodable`.

- Encodable

  Conforms when `Element` conforms to `Encodable`.

- Equatable

  Conforms when `Element` conforms to `Hashable`.

- ExpressibleByArrayLiteral

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- Hashable

  Conforms when `Element` conforms to `Hashable`.

- MutableCollection

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- MutableDataProtocol
- RandomAccessCollection

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- RangeReplaceableCollection

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- Sendable

  Conforms when `Element` conforms to `Copyable`, `Escapable`, and `Sendable`.

- Sequence

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

## See Also

### Related Array Types

struct ArraySlice

A slice of an `Array`, `ContiguousArray`, or `ArraySlice` instance.

