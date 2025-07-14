

- XPC
-  xpc_string_get_length(\_:) 

Function

# xpc_string_get_length(\_:)

Returns the length of the underlying string.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+

``` source
func xpc_string_get_length(_ xstring: xpc_object_t) -> Int
```

## Parameters 

`xstring`  

The string object which is to be examined.

## Return Value

The length of the underlying string, not including the `NULL`-terminator.

## See Also

### String objects

func xpc_string_create(UnsafePointer&lt;CChar>) -> xpc_object_t

Creates an XPC object that represents a null-terminated C-string.

func xpc_string_create_with_format_and_arguments(UnsafePointer&lt;CChar>, CVaListPointer) -> xpc_object_t

Creates an XPC object that represents a C-string that the specified format string and argument list pointer generate.

func xpc_string_get_string_ptr(xpc_object_t) -> UnsafePointer&lt;CChar>?

Returns a pointer to the internal storage of a string object.

