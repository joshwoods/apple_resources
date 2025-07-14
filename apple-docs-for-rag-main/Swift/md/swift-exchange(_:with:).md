

- Swift
-  exchange(\_:with:) 

Function

# exchange(\_:with:)

Replaces the value of a mutable value with the supplied new value, returning the original.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func exchange(
    _ item: inout T,
    with newValue: consuming T
) -> T where T : ~Copyable
```

## Parameters 

`item`  

A mutable binding.

`newValue`  

The new value of `item`.

## Return Value

The original value of `item`.

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

func withUnsafeTemporaryAllocation&lt;R>(byteCount: Int, alignment: Int, (UnsafeMutableRawBufferPointer) throws -> R) rethrows -> R

Provides scoped access to a raw buffer pointer with the specified byte count and alignment.

func swap&lt;T>(inout T, inout T)

Exchanges the values of the two arguments.

