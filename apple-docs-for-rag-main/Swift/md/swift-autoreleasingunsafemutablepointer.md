

- Swift
-  AutoreleasingUnsafeMutablePointer 

Structure

# AutoreleasingUnsafeMutablePointer

A mutable pointer addressing an Objective-C reference that doesn’t own its target.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct AutoreleasingUnsafeMutablePointer
```

## Mentioned in 

Using Imported C Functions in Swift

## Overview

`Pointee` must be a class type or `Optional` where `C` is a class.

This type has implicit conversions to allow passing any of the following to a C or ObjC API:

- `nil`, which gets passed as a null pointer,

- an inout argument of the referenced type, which gets passed as a pointer to a writeback temporary with autoreleasing ownership semantics,

- an `UnsafeMutablePointer`, which is passed as-is.

Passing pointers to mutable arrays of ObjC class pointers is not directly supported. Unlike `UnsafeMutablePointer`, `AutoreleasingUnsafeMutablePointer` must reference storage that does not own a reference count to the referenced value. UnsafeMutablePointer’s operations, by contrast, assume that the referenced storage owns values loaded from or stored to it.

This type does not carry an owner pointer unlike the other C\*Pointer types because it only needs to reference the results of inout conversions, which already have writeback-scoped lifetime.

## Topics

### Converting Pointers

init?&lt;U>(UnsafeMutablePointer&lt;U>?)

Explicit construction from an UnsafeMutablePointer.

init&lt;U>(UnsafeMutablePointer&lt;U>)

Explicit construction from an UnsafeMutablePointer.

### Accessing a Pointer’s Memory

var pointee: Pointee

Retrieve or set the `Pointee` instance referenced by `self`.

subscript(Int) -> Pointee

Access the `i`th element of the raw array pointed to by `self`.

### Comparing Pointers

static func == (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Instance Properties

var hashValue: Int

The hash value.

### Type Aliases

typealias Stride

A type that represents the distance between two values.

### Default Implementations

Comparable Implementations

CustomReflectable Implementations

Equatable Implementations

Hashable Implementations

Strideable Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- CVarArg

  Conforms when `Pointee` conforms to `Copyable` and `Escapable`.

- Comparable
- Copyable

  Conforms when `Pointee` conforms to `Copyable` and `Escapable`.

- CustomDebugStringConvertible
- CustomReflectable
- Equatable
- Hashable
- Strideable

## See Also

### C and Objective-C Pointers

struct OpaquePointer

A wrapper around an opaque C pointer.

