

- XPC
-  xpc_string_get_string_ptr(\_:) 

Function

# xpc_string_get_string_ptr(\_:)

Returns a pointer to the internal storage of a string object.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+

``` source
func xpc_string_get_string_ptr(_ xstring: xpc_object_t) -> UnsafePointer?
```

## Parameters 

`xstring`  

The string object which is to be examined.

## Return Value

A pointer to the string object’s internal storage.

## See Also

### String objects

func xpc_string_create(UnsafePointer&lt;CChar>) -> xpc_object_t

Creates an XPC object that represents a null-terminated C-string.

func xpc_string_create_with_format_and_arguments(UnsafePointer&lt;CChar>, CVaListPointer) -> xpc_object_t

Creates an XPC object that represents a C-string that the specified format string and argument list pointer generate.

func xpc_string_get_length(xpc_object_t) -> Int

Returns the length of the underlying string.

