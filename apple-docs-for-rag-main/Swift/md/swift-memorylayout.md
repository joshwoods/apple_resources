

- Swift
-  MemoryLayout 

Enumeration

# MemoryLayout

The memory layout of a type, describing its size, stride, and alignment.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
enum MemoryLayout where T : ~Copyable
```

## Overview

You can use `MemoryLayout` as a source of information about a type when allocating or binding memory using raw pointers. The following example declares a `Point` type with `x` and `y` coordinates and a Boolean `isFilled` property.

```
struct Point {
    let x: Double
    let y: Double
    let isFilled: Bool
}
```

The size, stride, and alignment of the `Point` type are accessible as static properties of `MemoryLayout`.

```
// MemoryLayout.size == 17
// MemoryLayout.stride == 24
// MemoryLayout.alignment == 8
```

Always use a multiple of a type’s `stride` instead of its `size` when allocating memory or accounting for the distance between instances in memory. This example allocates uninitialized raw memory with space for four instances of `Point`.

```
let count = 4
let pointPointer = UnsafeMutableRawPointer.allocate(
        byteCount: count * MemoryLayout.stride,
        alignment: MemoryLayout.alignment)
```

## Topics

### Accessing the Layout of a Type

Use these static properties to access a type’s layout. For example, the size of a `Double` instance is `MemoryLayout.size`.

static var size: Int

The contiguous memory footprint of `T`, in bytes.

static var alignment: Int

The default memory alignment of `T`, in bytes.

static var stride: Int

The number of bytes from the start of one instance of `T` to the start of the next when stored in contiguous memory or in an `Array`.

### Accessing the Layout of a Value

Pass an instance to these static methods to acess the layout for that instance’s type.

static func stride(ofValue: borrowing T) -> Int

Returns the number of bytes from the start of one instance of `T` to the start of the next when stored in contiguous memory or in an `Array`.

static func size(ofValue: borrowing T) -> Int

Returns the contiguous memory footprint of the given instance.

static func alignment(ofValue: borrowing T) -> Int

Returns the default memory alignment of `T`.

### Querying Type Properties

static func offset(of: PartialKeyPath&lt;T>) -> Int?

Returns the offset of an inline stored property within a type’s in-memory representation.

## Relationships

### Conforms To

- Sendable

  Conforms when `T` conforms to `Copyable` and `Escapable`.

