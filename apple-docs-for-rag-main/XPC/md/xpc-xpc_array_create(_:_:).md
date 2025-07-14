

- XPC
-  xpc_array_create(\_:\_:) 

Function

# xpc_array_create(\_:\_:)

Creates an XPC object that represents an array of XPC objects.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+

``` source
func xpc_array_create(
    _ objects: UnsafePointer?,
    _ count: Int
) -> xpc_object_t
```

## Parameters 

`objects`  

An array of XPC objects which is to be boxed. The order of this array is preserved in the object. If this array contains a NULL value, the behavior is undefined. This parameter may be NULL only if the count is 0.

`count`  

The number of objects in the given array. If the number passed is less than the actual number of values in the array, only the specified number of items are inserted into the resulting array. If the number passed is more than the the actual number of values, the behavior is undefined.

## Return Value

A new array object.

## Discussion

This array must be contiguous and cannot contain any NULL values. If you wish to insert the equivalent of a NULL value, you may use the result of xpc_null_create().

## See Also

### Array objects

struct XPCArray

An ordered random-access collection of XPC objects.

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

