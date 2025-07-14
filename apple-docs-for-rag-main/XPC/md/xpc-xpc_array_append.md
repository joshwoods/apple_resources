

- XPC
-  XPC_ARRAY_APPEND 

Global Variable

# XPC_ARRAY_APPEND

A constant to pass as the destination index to the class of primitive XPC array setters indicating that the specified primitive needs to append to the array.

iOS 8.0+iPadOS 8.0+Mac CatalystmacOS 10.10+tvOS 9.0+watchOS 2.0+

``` source
var XPC_ARRAY_APPEND: size_t { get }
```

## See Also

### Array objects

struct XPCArray

An ordered random-access collection of XPC objects.

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

