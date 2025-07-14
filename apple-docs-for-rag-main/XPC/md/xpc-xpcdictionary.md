

- XPC
-  XPCDictionary 

Structure

# XPCDictionary

A type that contains key-value pairs, notably used as the container of messages between a client and listener.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+watchOS 9.0+

``` source
struct XPCDictionary
```

## Topics

### Creating a dictionary

init()

Creates an empty dictionary.

init(xpc_object_t)

Creates a dictionary using the keys and values in the specified object parameter.

func copy(into: XPCDictionary)

Copies the keys and values of the dictionary to a different dictionary.

### Replying to client messages

func reply(XPCDictionary)

Sends a reply to the originator of the dictionary.

### Inspecting a dictionary

var isEmpty: Bool

A Boolean value that indicates whether the dictionary is empty.

var count: Int

The number of key-value pairs in the dictionary.

### Accessing keys and values

var keys: [String]

A collection containing just the keys of the dictionary.

var values: [xpc_object_t]

A collection containing just the values of the dictionary.

subscript(String) -> XPCDictionary?

Reads and writes the value associated with the given key as an XPC dictionary.

subscript(String) -> String?

Reads and writes the value associated with the given key as a string.

subscript(String) -> Bool?

Reads and writes the value associated with the given key as a Boolean value.

subscript(String) -> xpc_object_t?

Reads and writes the value associated with the given key as an XPC object.

subscript&lt;T>(String) -> T?

Reads and writes the value associated with the given key as a floating point value.

subscript&lt;T>(String) -> T?

Reads and writes the value associated with the given key as an unsigned integer value.

subscript&lt;T>(String) -> T?

Reads and writes the value associated with the given key as a signed integer value.

subscript(String, as _: XPCDictionary.Type) -> XPCDictionary?

Reads the value associated with the given key as an XPC dictionary.

subscript(String, as _: String.Type) -> String?

Reads and writes the value associated with the given key as a string.

subscript(String, as _: Bool.Type) -> Bool?

Reads and writes the value associated with the given key as a Boolean value.

subscript(String, as _: any OS_xpc_object.Type) -> xpc_object_t?

Reads and writes the value associated with the given key as an XPC object.

subscript(String, as _: xpc_type_t) -> xpc_object_t?

Reads and writes the value associated with the given key as an XPC object.

subscript&lt;T>(String, as _: T.Type) -> T?

Reads and writes the value associated with the given key as a floating point value.

subscript&lt;T>(String, as _: T.Type) -> T?

Reads and writes the value associated with the given key as an integer value.

subscript(String, as _: Bool.Type, default _: @autoclosure () -> Bool) -> Bool

Reads and writes the value associated with the given key as a Boolean value, falling back to the given default value.

subscript&lt;T>(String, as _: T.Type, default _: @autoclosure () -> T) -> T

Reads and writes the value associated with the given key converted to the specified type, falling back to the given default value.

func withUnsafeUnderlyingDictionary&lt;ReturnType>((xpc_object_t) throws -> ReturnType) rethrows -> ReturnType

Calls a closure with an unsafe reference to the dictionary.

### Removing keys and values

func removeValue(forKey: String) -> xpc_object_t?

Removes the given key and its associated value from the dictionary.

### Supporting types

typealias KeyValuePair

A type that contains a dictionary’s key-value pair.

### Iterating over keys and values

func forEach((XPCDictionary.KeyValuePair) throws -> Void) rethrows

Calls the given closure with each element in the dictionary in the same order as a for-in loop.

func forEach((String, xpc_object_t) throws -> Void) rethrows

Calls the given closure with each key and value in the dictionary in the same order as a for-in loop.

### Transforming a dictionary

func map&lt;ReturnType>((XPCDictionary.KeyValuePair) throws -> ReturnType) rethrows -> [ReturnType]

Returns an array containing the results of mapping the given closure over the sequence’s elements.

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- Equatable
- Hashable

## See Also

### Dictionary objects

func xpc_dictionary_create(UnsafePointer&lt;UnsafePointer&lt;CChar>>?, UnsafePointer&lt;xpc_object_t?>?, Int) -> xpc_object_t

Creates an XPC object that represents a dictionary of XPC objects keyed to C-strings.

func xpc_dictionary_create_empty() -> xpc_object_t

Creates an XPC object that represents a dictionary of XPC objects keyed to C-strings.

func xpc_dictionary_create_connection(xpc_object_t, UnsafePointer&lt;CChar>) -> xpc_connection_t?

Creates a connection from a dictionary directly.

func xpc_dictionary_create_reply(xpc_object_t) -> xpc_object_t?

Creates a dictionary that is in reply to the specified dictionary.

func xpc_dictionary_set_value(xpc_object_t, UnsafePointer&lt;CChar>, xpc_object_t?)

Sets the value for the specified key to the specified object.

func xpc_dictionary_get_count(xpc_object_t) -> Int

Returns the number of values in the dictionary.

func xpc_dictionary_get_value(xpc_object_t, UnsafePointer&lt;CChar>) -> xpc_object_t?

Returns the value for the specified key.

func xpc_dictionary_apply(xpc_object_t, (UnsafePointer&lt;CChar>, xpc_object_t) -> Bool) -> Bool

Invokes the specified block for every key-value pair in the dictionary.

func xpc_dictionary_dup_fd(xpc_object_t, UnsafePointer&lt;CChar>) -> Int32

Creates a file descriptor from a dictionary directly.

func xpc_dictionary_get_array(xpc_object_t, UnsafePointer&lt;CChar>) -> xpc_object_t?

Returns the array value for the specified key.

func xpc_dictionary_get_bool(xpc_object_t, UnsafePointer&lt;CChar>) -> Bool

Gets a Boolean primitive value from a dictionary directly.

func xpc_dictionary_get_data(xpc_object_t, UnsafePointer&lt;CChar>, UnsafeMutablePointer&lt;Int>?) -> UnsafeRawPointer?

Gets a raw data value from a dictionary directly.

func xpc_dictionary_get_date(xpc_object_t, UnsafePointer&lt;CChar>) -> Int64

Gets a date value from a dictionary directly.

func xpc_dictionary_get_dictionary(xpc_object_t, UnsafePointer&lt;CChar>) -> xpc_object_t?

Returns the dictionary value for the specified key.

func xpc_dictionary_get_double(xpc_object_t, UnsafePointer&lt;CChar>) -> Double

Gets a double-precision floating point primitive value from a dictionary directly.

