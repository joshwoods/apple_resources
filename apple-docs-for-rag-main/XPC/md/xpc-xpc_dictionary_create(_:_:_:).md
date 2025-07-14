

- XPC
-  xpc_dictionary_create(\_:\_:\_:) 

Function

# xpc_dictionary_create(\_:\_:\_:)

Creates an XPC object that represents a dictionary of XPC objects keyed to C-strings.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+

``` source
func xpc_dictionary_create(
    _ keys: UnsafePointer>?,
    _ values: UnsafePointer?,
    _ count: Int
) -> xpc_object_t
```

## Parameters 

`keys`  

An array of C-strings that are to be the keys for the values to be inserted. Each element of this array is copied into the dictionary’s internal storage. If any element of this array is NULL, the behavior is undefined.

`values`  

A C-array that is parallel to the array of keys, consisting of objects that are to be inserted. Each element in this array is retained. Elements in this array may be NULL.

`count`  

The number of key/value pairs in the given arrays. If the count is less than the actual count of values, only that many key/value pairs will be inserted into the dictionary.

If the count is more than the the actual count of key/value pairs, the behavior is undefined. If one array is NULL and the other is not, the behavior is undefined. If both arrays are NULL and the count is non-0, the behavior is undefined.

## Return Value

The new dictionary object.

## See Also

### Dictionary objects

struct XPCDictionary

A type that contains key-value pairs, notably used as the container of messages between a client and listener.

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

