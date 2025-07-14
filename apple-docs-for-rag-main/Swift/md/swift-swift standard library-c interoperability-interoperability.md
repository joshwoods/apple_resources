

- Swift
- Swift Standard Library
-  C Interoperability 

API Collection

# C Interoperability

Use imported C types or call C variadic functions.

## Topics

### C and Objective-C Pointers

struct OpaquePointer

A wrapper around an opaque C pointer.

struct AutoreleasingUnsafeMutablePointer

A mutable pointer addressing an Objective-C reference that doesn’t own its target.

### C Variadic Functions

func withVaList&lt;R>([any CVarArg], (CVaListPointer) -> R) -> R

Invokes the given closure with a C `va_list` argument derived from the given array of arguments.

struct CVaListPointer

protocol CVarArg

A type whose instances can be encoded, and appropriately passed, as elements of a C `va_list`.

func getVaList([any CVarArg]) -> CVaListPointer

Returns a `CVaListPointer` that is backed by autoreleased storage, built from the given array of arguments.

### Pointers to Values

Access a pointer to a variable in memory for explicit passing to C functions.

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

### Aliases for Imported C Types

typealias CBool

The C ‘\_Bool’ and C++ ‘bool’ type.

typealias CChar

The C ‘char’ type.

typealias CChar16

The C++11 ‘char16_t’ type, which has UTF-16 encoding.

typealias CChar32

The C++11 ‘char32_t’ type, which has UTF-32 encoding.

typealias CDouble

The C ‘double’ type.

typealias CLongDouble

typealias CFloat

The C ‘float’ type.

typealias CFloat16

The C ‘\_Float16’ type.

typealias CInt

typealias CLong

typealias CLongLong

The C ‘long long’ type.

typealias CShort

The C ‘short’ type.

typealias CSignedChar

The C ‘signed char’ type.

typealias CUnsignedChar

The C ‘unsigned char’ type.

typealias CUnsignedInt

typealias CUnsignedLong

typealias CUnsignedLongLong

The C ‘unsigned long long’ type.

typealias CUnsignedShort

The C ‘unsigned short’ type.

typealias CWideChar

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

Manual Memory Management

Allocate and manage memory manually.

Type Casting and Existential Types

Perform casts between types or represent values of any type.

Operator Declarations

Work with prefix, postfix, and infix operators.

