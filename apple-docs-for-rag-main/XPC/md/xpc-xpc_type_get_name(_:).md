

- XPC
-  xpc_type_get_name(\_:) 

Function

# xpc_type_get_name(\_:)

Returns a string that describes an XPC object type.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+

``` source
func xpc_type_get_name(_ type: xpc_type_t) -> UnsafePointer
```

## Parameters 

`type`  

The type to describe.

## Return Value

A string describing the type of an object, like `"string"` or `"int64"`. This string should not be freed or modified.

## See Also

### Identity

func xpc_get_type(xpc_object_t) -> xpc_type_t

Returns the type of an object.

func xpc_hash(xpc_object_t) -> Int

Calculates a hash value for the specified object.

