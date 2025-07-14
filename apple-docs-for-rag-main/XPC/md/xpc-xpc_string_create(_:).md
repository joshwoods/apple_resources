

- XPC
-  xpc_string_create(\_:) 

Function

# xpc_string_create(\_:)

Creates an XPC object that represents a null-terminated C-string.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+

``` source
func xpc_string_create(_ string: UnsafePointer) -> xpc_object_t
```

## Parameters 

`string`  

The C-string which is to be boxed.

## Return Value

A new string object.

## See Also

### String objects

func xpc_string_create_with_format_and_arguments(UnsafePointer&lt;CChar>, CVaListPointer) -> xpc_object_t

Creates an XPC object that represents a C-string that the specified format string and argument list pointer generate.

func xpc_string_get_length(xpc_object_t) -> Int

Returns the length of the underlying string.

func xpc_string_get_string_ptr(xpc_object_t) -> UnsafePointer&lt;CChar>?

Returns a pointer to the internal storage of a string object.

