

- Swift
-  OpaquePointer 

Structure

# OpaquePointer

A wrapper around an opaque C pointer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct OpaquePointer
```

## Overview

Opaque pointers are used to represent C pointers to types that cannot be represented in Swift, such as incomplete struct types.

## Topics

### Initializers

init(UnsafeRawPointer)

init?(UnsafeMutableRawPointer?)

init&lt;T>(UnsafePointer&lt;T>)

Converts a typed `UnsafePointer` to an opaque C pointer.

init?(UnsafeRawPointer?)

init&lt;T>(UnsafeMutablePointer&lt;T>)

Converts a typed `UnsafeMutablePointer` to an opaque C pointer.

init(UnsafeMutableRawPointer)

init?&lt;T>(UnsafePointer&lt;T>?)

Converts a typed `UnsafePointer` to an opaque C pointer.

init?&lt;T>(UnsafeMutablePointer&lt;T>?)

Converts a typed `UnsafeMutablePointer` to an opaque C pointer.

init?(bitPattern: Int)

Creates a new `OpaquePointer` from the given address, specified as a bit pattern.

init?(bitPattern: UInt)

Creates a new `OpaquePointer` from the given address, specified as a bit pattern.

### Default Implementations

AtomicOptionalRepresentable Implementations

AtomicRepresentable Implementations

CustomDebugStringConvertible Implementations

Equatable Implementations

Hashable Implementations

## Relationships

### Conforms To

- AtomicOptionalRepresentable
- AtomicRepresentable
- BitwiseCopyable
- CVarArg
- Copyable
- CustomDebugStringConvertible
- Equatable
- Hashable

## See Also

### C and Objective-C Pointers

struct AutoreleasingUnsafeMutablePointer

A mutable pointer addressing an Objective-C reference that doesn’t own its target.

