

- Swift
- Swift Standard Library
-  Manual Memory Management 

API Collection

# Manual Memory Management

Allocate and manage memory manually.

## Topics

### First Steps

Calling Functions With Pointer Parameters

Use implicit pointer casting or bridging when calling functions that takes pointers as parameters.

### Typed Pointers

Use typed pointers and buffers to access memory as instances of a specific type.

struct UnsafePointer

A pointer for accessing data of a specific type.

struct UnsafeMutablePointer

A pointer for accessing and manipulating data of a specific type.

struct UnsafeBufferPointer

A nonowning collection interface to a buffer of elements stored contiguously in memory.

struct UnsafeMutableBufferPointer

A nonowning collection interface to a buffer of mutable elements stored contiguously in memory.

### Raw Pointers

Use raw pointers and buffers to access memory for loading and storing as raw bytes.

struct UnsafeRawPointer

A raw pointer for accessing untyped data.

struct UnsafeMutableRawPointer

A raw pointer for accessing and manipulating untyped data.

struct UnsafeRawBufferPointer

A nonowning collection interface to the bytes in a region of memory.

struct UnsafeMutableRawBufferPointer

A mutable nonowning collection interface to the bytes in a region of memory.

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

func exchange&lt;T>(inout T, with: consuming T) -> T

Replaces the value of a mutable value with the supplied new value, returning the original.

### Memory Layout

enum MemoryLayout

The memory layout of a type, describing its size, stride, and alignment.

### Reference Counting

struct Unmanaged

A type for propagating an unmanaged object reference.

func withExtendedLifetime&lt;T, E, Result>(borrowing T, (borrowing T) throws(E) -> Result) throws(E) -> Result

Evaluates a closure while ensuring that the given instance is not destroyed before the closure returns.

func withExtendedLifetime&lt;T, E, Result>(borrowing T, () throws(E) -> Result) throws(E) -> Result

Evaluates a closure while ensuring that the given instance is not destroyed before the closure returns.

## See Also

### Programming Tasks

Input and Output

Print values to the console, read from and write to text streams, and use command line arguments.

Debugging and Reflection

Fortify your code with runtime checks, and examine your values’ runtime representation.

Macros

Generate boilerplate code and perform other compile-time operations.

Concurrency

Perform asynchronous and parallel operations.

Key-Path Expressions

Use key-path expressions to access properties dynamically.

Type Casting and Existential Types

Perform casts between types or represent values of any type.

C Interoperability

Use imported C types or call C variadic functions.

Operator Declarations

Work with prefix, postfix, and infix operators.

