

- Swift
-  UnsafeRawPointer 

Structure

# UnsafeRawPointer

A raw pointer for accessing untyped data.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct UnsafeRawPointer
```

## Mentioned in 

Using Imported C Functions in Swift

## Overview

The `UnsafeRawPointer` type provides no automated memory management, no type safety, and no alignment guarantees. You are responsible for handling the life cycle of any memory you work with through unsafe pointers, to avoid leaks or undefined behavior.

Memory that you manually manage can be either *untyped* or *bound* to a specific type. You use the `UnsafeRawPointer` type to access and manage raw bytes in memory, whether or not that memory has been bound to a specific type.

# Understanding a Pointer’s Memory State

The memory referenced by an `UnsafeRawPointer` instance can be in one of several states. Many pointer operations must only be applied to pointers with memory in a specific state—you must keep track of the state of the memory you are working with and understand the changes to that state that different operations perform. Memory can be untyped and uninitialized, bound to a type and uninitialized, or bound to a type and initialized to a value. Finally, memory that was allocated previously may have been deallocated, leaving existing pointers referencing unallocated memory.

## Raw, Uninitialized Memory

Raw memory that has just been allocated is in an *uninitialized, untyped* state. Uninitialized memory must be initialized with values of a type before it can be used with any typed operations.

To bind uninitialized memory to a type without initializing it, use the `bindMemory(to:count:)` method. This method returns a typed pointer for further typed access to the memory.

## Typed Memory

Memory that has been bound to a type, whether it is initialized or uninitialized, is typically accessed using typed pointers—instances of `UnsafePointer` and `UnsafeMutablePointer`. Initialization, assignment, and deinitialization can be performed using `UnsafeMutablePointer` methods.

Memory that has been bound to a type can be rebound to a different type only after it has been deinitialized or if the bound type is a *trivial type*. Deinitializing typed memory does not unbind that memory’s type. The deinitialized memory can be reinitialized with values of the same type, bound to a new type, or deallocated.

Note

A trivial type can be copied bit for bit with no indirection or reference-counting operations. Generally, native Swift types that do not contain strong or weak references or other forms of indirection are trivial, as are imported C structs and enumerations.

When reading from memory as raw bytes when that memory is bound to a type, you must ensure that you satisfy any alignment requirements.

# Raw Pointer Arithmetic

Pointer arithmetic with raw pointers is performed at the byte level. When you add to or subtract from a raw pointer, the result is a new raw pointer offset by that number of bytes. The following example allocates four bytes of memory and stores `0xFF` in all four bytes:

```
let bytesPointer = UnsafeMutableRawPointer.allocate(byteCount: 4, alignment: 4)
bytesPointer.storeBytes(of: 0xFFFF_FFFF, as: UInt32.self)

// Load a value from the memory referenced by 'bytesPointer'
let x = bytesPointer.load(as: UInt8.self)       // 255

// Load a value from the last two allocated bytes
let offsetPointer = bytesPointer + 2
let y = offsetPointer.load(as: UInt16.self)     // 65535
```

The code above stores the value `0xFFFF_FFFF` into the four newly allocated bytes, and then loads the first byte as a `UInt8` instance and the third and fourth bytes as a `UInt16` instance.

Always remember to deallocate any memory that you allocate yourself.

```
bytesPointer.deallocate()
```

# Implicit Casting and Bridging

When calling a function or method with an `UnsafeRawPointer` parameter, you can pass an instance of that specific pointer type, pass an instance of a compatible pointer type, or use Swift’s implicit bridging to pass a compatible pointer.

For example, the `print(address:as:)` function in the following code sample takes an `UnsafeRawPointer` instance as its first parameter:

```
func print(address p: UnsafeRawPointer, as type: T.Type) {
    let value = p.load(as: type)
    print(value)
}
```

As is typical in Swift, you can call the `print(address:as:)` function with an `UnsafeRawPointer` instance. This example passes `rawPointer` as the initial parameter.

```
// 'rawPointer' points to memory initialized with `Int` values.
let rawPointer: UnsafeRawPointer = ...
print(address: rawPointer, as: Int.self)
// Prints "42"
```

Because typed pointers can be implicitly cast to raw pointers when passed as a parameter, you can also call `print(address:as:)` with any mutable or immutable typed pointer instance.

```
let intPointer: UnsafePointer = ...
print(address: intPointer, as: Int.self)
// Prints "42"

let mutableIntPointer = UnsafeMutablePointer(mutating: intPointer)
print(address: mutableIntPointer, as: Int.self)
// Prints "42"
```

Alternatively, you can use Swift’s *implicit bridging* to pass a pointer to an instance or to the elements of an array. Use inout syntax to implicitly create a pointer to an instance of any type. The following example uses implicit bridging to pass a pointer to `value` when calling `print(address:as:)`:

```
var value: Int = 23
print(address: &value, as: Int.self)
// Prints "23"
```

An immutable pointer to the elements of an array is implicitly created when you pass the array as an argument. This example uses implicit bridging to pass a pointer to the elements of `numbers` when calling `print(address:as:)`.

```
let numbers = [5, 10, 15, 20]
print(address: numbers, as: Int.self)
// Prints "5"
```

You can also use inout syntax to pass a mutable pointer to the elements of an array. Because `print(address:as:)` requires an immutable pointer, although this is syntactically valid, it isn’t necessary.

```
var mutableNumbers = numbers
print(address: &mutableNumbers, as: Int.self)
```

Important

The pointer created through implicit bridging of an instance or of an array’s elements is only valid during the execution of the called function. Escaping the pointer to use after the execution of the function is undefined behavior. In particular, do not use implicit bridging when calling an `UnsafeRawPointer` initializer.

```
var number = 5
let numberPointer = UnsafeRawPointer(&number)
// Accessing 'numberPointer' is undefined behavior.
```

## Topics

### Initializers

init&lt;T>(AutoreleasingUnsafeMutablePointer&lt;T>)

Creates a new raw pointer from an `AutoreleasingUnsafeMutablePointer` instance.

init?&lt;T>(UnsafePointer&lt;T>?)

Creates a new raw pointer from the given typed pointer.

init?&lt;T>(AutoreleasingUnsafeMutablePointer&lt;T>?)

Creates a new raw pointer from an `AutoreleasingUnsafeMutablePointer` instance.

init?(UnsafeMutableRawPointer?)

Creates a new raw pointer from the given mutable raw pointer.

init?&lt;T>(UnsafeMutablePointer&lt;T>?)

Creates a new raw pointer from the given typed pointer.

init&lt;T>(UnsafePointer&lt;T>)

Creates a new raw pointer from the given typed pointer.

init(UnsafeMutableRawPointer)

Creates a new raw pointer from the given mutable raw pointer.

init&lt;T>(UnsafeMutablePointer&lt;T>)

Creates a new raw pointer from the given typed pointer.

### Instance Properties

var customPlaygroundQuickLook: _PlaygroundQuickLook

A custom playground Quick Look for this instance.

var hashValue: Int

The hash value.

### Instance Methods

func alignedDown&lt;T>(for: T.Type) -> UnsafeRawPointer

Obtain the preceding pointer properly aligned to store a value of type `T`.

func alignedDown(toMultipleOf: Int) -> UnsafeRawPointer

Obtain the preceding pointer whose bit pattern is a multiple of `alignment`.

func alignedUp&lt;T>(for: T.Type) -> UnsafeRawPointer

Obtain the next pointer properly aligned to store a value of type `T`.

func alignedUp(toMultipleOf: Int) -> UnsafeRawPointer

Obtain the next pointer whose bit pattern is a multiple of `alignment`.

func assumingMemoryBound&lt;T>(to: T.Type) -> UnsafePointer&lt;T>

Returns a typed pointer to the memory referenced by this pointer, assuming that the memory is already bound to the specified type.

func bindMemory&lt;T>(to: T.Type, capacity: Int) -> UnsafePointer&lt;T>

Binds the memory to the specified type and returns a typed pointer to the bound memory.

func deallocate()

Deallocates the previously allocated memory block referenced by this pointer.

func load&lt;T>(fromByteOffset: Int, as: T.Type) -> T

Returns a new instance of the given type, constructed from the raw memory at the specified offset.

func loadUnaligned&lt;T>(fromByteOffset: Int, as: T.Type) -> T

Returns a new instance of the given type, constructed from the raw memory at the specified offset.

func loadUnaligned&lt;T>(fromByteOffset: Int, as: T.Type) -> T

Returns a new instance of the given type, constructed from the raw memory at the specified offset.

func withMemoryRebound&lt;T, E, Result>(to: T.Type, capacity: Int, (UnsafePointer&lt;T>) throws(E) -> Result) throws(E) -> Result

Executes the given closure while temporarily binding memory to the specified number of instances of type `T`.

### Type Aliases

typealias Pointee

### Default Implementations

AtomicOptionalRepresentable Implementations

AtomicRepresentable Implementations

Comparable Implementations

CustomReflectable Implementations

Equatable Implementations

Hashable Implementations

Strideable Implementations

## Relationships

### Conforms To

- AtomicOptionalRepresentable
- AtomicRepresentable
- BitwiseCopyable
- Comparable
- Copyable
- CustomDebugStringConvertible
- CustomReflectable
- Equatable
- Hashable
- Strideable

## See Also

### Raw Pointers

struct UnsafeMutableRawPointer

A raw pointer for accessing and manipulating untyped data.

struct UnsafeRawBufferPointer

A nonowning collection interface to the bytes in a region of memory.

struct UnsafeMutableRawBufferPointer

A mutable nonowning collection interface to the bytes in a region of memory.

