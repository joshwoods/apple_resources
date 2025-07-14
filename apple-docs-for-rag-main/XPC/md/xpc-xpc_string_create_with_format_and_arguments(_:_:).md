

- XPC
-  xpc_string_create_with_format_and_arguments(\_:\_:) 

Function

# xpc_string_create_with_format_and_arguments(\_:\_:)

Creates an XPC object that represents a C-string that the specified format string and argument list pointer generate.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+

``` source
func xpc_string_create_with_format_and_arguments(
    _ fmt: UnsafePointer,
    _ ap: CVaListPointer
) -> xpc_object_t
```

## Parameters 

`fmt`  

The `printf(3)`-style format string from which to construct the final C-string to be boxed.

`ap`  

A pointer to the arguments which correspond to those specified in the format string.

## Return Value

A new string object.

## See Also

### String objects

func xpc_string_create(UnsafePointer&lt;CChar>) -> xpc_object_t

Creates an XPC object that represents a null-terminated C-string.

func xpc_string_get_length(xpc_object_t) -> Int

Returns the length of the underlying string.

func xpc_string_get_string_ptr(xpc_object_t) -> UnsafePointer&lt;CChar>?

Returns a pointer to the internal storage of a string object.

