

- XPC
-  XPCArray 

Structure

# XPCArray

An ordered random-access collection of XPC objects.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+watchOS 9.0+

``` source
struct XPCArray
```

## Topics

### Creating an array

init()

Creates a new, empty array.

init(xpc_object_t)

Creates a new array that contains the given XPC object.

func copy(into: XPCArray)

Copies the elements of the array to a different array.

### Inspecting an array

var isEmpty: Bool

A Boolean value that indicates whether the array is empty.

var count: Int

The number of elements in the array.

### Accessing elements

subscript(Int) -> XPCDictionary?

Reads and writes the value at the given index as an XPC dictionary.

subscript(Int) -> String?

Reads and writes the value at the given index as a string.

subscript(Int) -> Bool?

Reads and writes the value at the given index as a Boolean value.

subscript(Int) -> xpc_object_t?

Reads and writes the value at the given index as an XPC object.

subscript&lt;T>(Int) -> T?

Reads and writes the value at the given index as a floating point value.

subscript&lt;T>(Int) -> T?

Reads and writes the value at the given index as an unsigned integer.

subscript&lt;T>(Int) -> T?

Reads and writes the value at the given index as a signed integer.

subscript(Int, as _: XPCDictionary.Type) -> XPCDictionary?

Reads the value associated with the given key as an XPC dictionary.

subscript(Int, as _: String.Type) -> String?

Reads and writes the value at the given index as a string.

subscript(Int, as _: Bool.Type) -> Bool?

Reads and writes the value at the given index as a Boolean value.

subscript(Int, as _: any OS_xpc_object.Type) -> xpc_object_t?

Reads and writes the value at the given index as an XPC object.

subscript(Int, as _: xpc_type_t) -> xpc_object_t?

Reads and writes the value at the given index as an XPC object.

subscript&lt;T>(Int, as _: T.Type) -> T?

Reads and writes the value at the given index as a floating point value.

subscript&lt;T>(Int, as _: T.Type) -> T?

Reads and writes the value at the given index as an integer value.

subscript(Int, as _: Bool.Type, default _: @autoclosure () -> Bool) -> Bool

Reads and writes the value at the given index as a Boolean value, falling back to the given default value.

subscript&lt;T>(Int, as _: T.Type, default _: @autoclosure () -> T) -> T

Reads and writes the value at the given index as a floating point value, falling back to the given default value.

func withUnsafeUnderlyingArray&lt;ReturnType>((xpc_object_t) throws -> ReturnType) rethrows -> ReturnType

Calls a closure with an unsafe reference to the array.

### Iterating over an array’s elements

func forEach((XPCArray.IndexValuePair) throws -> Void) rethrows

Calls the given closure with each element in the array in the same order as a for-in loop.

func forEach((Int, xpc_object_t) throws -> Void) rethrows

Calls the given closure with an index and element of the array in the same order as a for-in loop.

### Transforming an array

func map&lt;ReturnType>((XPCArray.IndexValuePair) throws -> ReturnType) rethrows -> [ReturnType]

Returns an array containing the results of mapping the given closure over the sequence’s elements.

### Supporting types

typealias IndexValuePair

A type that contains an index and the object at that index.

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- Equatable
- Hashable

## See Also

### Array objects

func xpc_array_create(UnsafePointer&lt;xpc_object_t>?, Int) -> xpc_object_t

Creates an XPC object that represents an array of XPC objects.

func xpc_array_create_empty() -> xpc_object_t

Creates an XPC object that represents an array of XPC objects.

func xpc_array_create_connection(xpc_object_t, Int) -> xpc_connection_t?

Creates a connection object from an array directly.

func xpc_array_set_value(xpc_object_t, Int, xpc_object_t)

Inserts the specified object into the array at the specified index.

func xpc_array_get_value(xpc_object_t, Int) -> xpc_object_t

Returns the value at the specified index in the array.

func xpc_array_append_value(xpc_object_t, xpc_object_t)

Appends an object to an XPC array.

func xpc_array_get_count(xpc_object_t) -> Int

Returns the count of values in the array.

func xpc_array_apply(xpc_object_t, (Int, xpc_object_t) -> Bool) -> Bool

Invokes the specified block for every value in the array.

func xpc_array_dup_fd(xpc_object_t, Int) -> Int32

Gets a file descriptor from an array directly.

func xpc_array_get_array(xpc_object_t, Int) -> xpc_object_t?

Returns the array at the specified index in the array.

func xpc_array_get_bool(xpc_object_t, Int) -> Bool

Gets a Boolean primitive value from an array directly.

func xpc_array_get_data(xpc_object_t, Int, UnsafeMutablePointer&lt;Int>?) -> UnsafeRawPointer?

Gets a pointer to the raw bytes of a data object from an array directly.

func xpc_array_get_date(xpc_object_t, Int) -> Int64

Gets a date interval from an array directly.

func xpc_array_get_dictionary(xpc_object_t, Int) -> xpc_object_t?

Returns the dictionary at the specified index in the array.

func xpc_array_get_double(xpc_object_t, Int) -> Double

Gets a double-precision floating point primitive value from an array directly.

