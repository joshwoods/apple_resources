

- XPC
-  xpc_uuid_get_bytes(\_:) 

Function

# xpc_uuid_get_bytes(\_:)

Copies the UUID that an XPC UUID object boxes into the specified UUID buffer.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+

``` source
func xpc_uuid_get_bytes(_ xuuid: xpc_object_t) -> UnsafePointer?
```

## Parameters 

`xuuid`  

The UUID object which is to be examined.

## Return Value

The underlying `uuid_t` bytes. The returned pointer may be safely passed to the `uuid(3)` APIs.

## See Also

### UUID objects

func xpc_uuid_create(UnsafePointer&lt;UInt8>) -> xpc_object_t

Creates an XPC object that represents a universally unique identifier (UUID).

