

- XPC
-  xpc_uuid_create(\_:) 

Function

# xpc_uuid_create(\_:)

Creates an XPC object that represents a universally unique identifier (UUID).

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+

``` source
func xpc_uuid_create(_ uuid: UnsafePointer) -> xpc_object_t
```

## Parameters 

`uuid`  

The UUID which is to be boxed.

## Return Value

A new UUID object.

## See Also

### UUID objects

func xpc_uuid_get_bytes(xpc_object_t) -> UnsafePointer&lt;UInt8>?

Copies the UUID that an XPC UUID object boxes into the specified UUID buffer.

