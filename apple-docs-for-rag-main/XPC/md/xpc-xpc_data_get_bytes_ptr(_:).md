

- XPC
-  xpc_data_get_bytes_ptr(\_:) 

Function

# xpc_data_get_bytes_ptr(\_:)

Returns a pointer to the internal storage of a data object.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+

``` source
func xpc_data_get_bytes_ptr(_ xdata: xpc_object_t) -> UnsafeRawPointer?
```

## Parameters 

`xdata`  

The data object which is to be examined.

## Return Value

A pointer to the underlying boxed data.

## See Also

### Data objects

func xpc_data_create(UnsafeRawPointer?, Int) -> xpc_object_t

Creates an XPC object that represents a buffer of bytes.

func xpc_data_create_with_dispatch_data(dispatch_data_t) -> xpc_object_t

Creates an XPC object that represents a buffer of bytes that the specified GCD data object describes.

func xpc_data_get_bytes(xpc_object_t, UnsafeMutableRawPointer, Int, Int) -> Int

Copies the bytes in a data object into the specified buffer.

func xpc_data_get_length(xpc_object_t) -> Int

Returns the length of the data that an XPC data object encapsulates.

