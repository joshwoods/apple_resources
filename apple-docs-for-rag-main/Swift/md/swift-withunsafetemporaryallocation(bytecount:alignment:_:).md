

- Swift
-  withUnsafeTemporaryAllocation(byteCount:alignment:\_:) 

Function

# withUnsafeTemporaryAllocation(byteCount:alignment:\_:)

Provides scoped access to a raw buffer pointer with the specified byte count and alignment.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func withUnsafeTemporaryAllocation(
    byteCount: Int,
    alignment: Int,
    _ body: (UnsafeMutableRawBufferPointer) throws -> R
) rethrows -> R where R : ~Copyable
```

## Parameters 

`byteCount`  

The number of bytes to temporarily allocate. `byteCount` must not be negative.

`alignment`  

The alignment of the new, temporary region of allocated memory, in bytes. `alignment` must be a whole power of 2.

`body`  

A closure to invoke and to which the allocated buffer pointer should be passed.

## Return Value

Whatever is returned by `body`.

## Discussion

Throws

Whatever is thrown by `body`.

This function is useful for cheaply allocating raw storage for a brief duration. Storage may be allocated on the heap or on the stack, depending on the required size and alignment.

When `body` is called, the contents of the buffer pointer passed to it are in an unspecified, uninitialized state. `body` is responsible for initializing the buffer pointer before it is used *and* for deinitializing it before returning, but deallocation is automatic.

The implementation may allocate a larger buffer pointer than is strictly necessary to contain `byteCount` bytes. The behavior of a program that attempts to access any such additional storage is undefined.

The buffer pointer passed to `body` (as well as any pointers to elements in the buffer) must not escape. It will be deallocated when `body` returns and cannot be used afterward.

## See Also

### Memory Access

func withUnsafePointer&lt;T, E, Result>(to: inout T, (UnsafePointer&lt;T>) throws(E) -> Result) throws(E) -> Result

Invokes the given closure with a pointer to the given argument.

func withUnsafePointer&lt;T, E, Result>(to: borrowing T, (UnsafePointer&lt;T>) throws(E) -> Result) throws(E) -> Result

Invokes the given closure with a pointer to the given argument.

func withUnsafeMutablePointer&lt;T, E, Result>(to: inout T, (UnsafeMutablePointer&lt;T>) throws(E) -> Result) throws(E) -> Result

Calls the given closure with a mutable pointer to the given argument.

func withUnsafeBytes&lt;T, E, Result>(of: inout T, (UnsafeRawBufferPointer) throws(E) -> Result) throws(E) -> Result

Invokes the given closure with a buffer pointer covering the raw bytes of the given argument.

func withUnsafeBytes&lt;T, E, Result>(of: borrowing T, (UnsafeRawBufferPointer) throws(E) -> Result) throws(E) -> Result

Invokes the given closure with a buffer pointer covering the raw bytes of the given argument.

func withUnsafeMutableBytes&lt;T, E, Result>(of: inout T, (UnsafeMutableRawBufferPointer) throws(E) -> Result) throws(E) -> Result

Invokes the given closure with a mutable buffer pointer covering the raw bytes of the given argument.

func withUnsafeTemporaryAllocation&lt;T, R>(of: T.Type, capacity: Int, (UnsafeMutableBufferPointer&lt;T>) throws -> R) rethrows -> R

Provides scoped access to a buffer pointer to memory of the specified type and with the specified capacity.

func swap&lt;T>(inout T, inout T)

Exchanges the values of the two arguments.

func exchange&lt;T>(inout T, with: consuming T) -> T

Replaces the value of a mutable value with the supplied new value, returning the original.

