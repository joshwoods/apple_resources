

- XPC
-  xpc_data_create(\_:\_:) 

Function

# xpc_data_create(\_:\_:)

Creates an XPC object that represents a buffer of bytes.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+

``` source
func xpc_data_create(
    _ bytes: UnsafeRawPointer?,
    _ length: Int
) -> xpc_object_t
```

## Parameters 

`bytes`  

The buffer of bytes which is to be boxed. You may create an empty data object by passing NULL for this parameter and 0 for the length. Passing NULL with any other length will result in undefined behavior.

`length`  

The number of bytes which are to be boxed.

## Return Value

A new data object.

## Discussion

This method will copy the buffer given into internal storage. After calling this method, it is safe to dispose of the given buffer.

## See Also

### Data objects

func xpc_data_create_with_dispatch_data(dispatch_data_t) -> xpc_object_t

Creates an XPC object that represents a buffer of bytes that the specified GCD data object describes.

func xpc_data_get_bytes(xpc_object_t, UnsafeMutableRawPointer, Int, Int) -> Int

Copies the bytes in a data object into the specified buffer.

func xpc_data_get_bytes_ptr(xpc_object_t) -> UnsafeRawPointer?

Returns a pointer to the internal storage of a data object.

func xpc_data_get_length(xpc_object_t) -> Int

Returns the length of the data that an XPC data object encapsulates.

