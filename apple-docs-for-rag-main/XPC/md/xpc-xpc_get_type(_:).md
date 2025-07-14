

- XPC
-  xpc_get_type(\_:) 

Function

# xpc_get_type(\_:)

Returns the type of an object.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+

``` source
func xpc_get_type(_ object: xpc_object_t) -> xpc_type_t
```

## Parameters 

`object`  

The object to examine.

## Return Value

An opaque pointer describing the type of the object. This pointer is suitable for direct comparison to exported type constants with the equality operator.

## See Also

### Identity

func xpc_type_get_name(xpc_type_t) -> UnsafePointer&lt;CChar>

Returns a string that describes an XPC object type.

func xpc_hash(xpc_object_t) -> Int

Calculates a hash value for the specified object.

