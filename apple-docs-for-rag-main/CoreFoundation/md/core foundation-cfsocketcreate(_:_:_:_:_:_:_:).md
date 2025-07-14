

- Core Foundation
-  CFSocketCreate(\_:\_:\_:\_:\_:\_:\_:) 

Function

# CFSocketCreate(\_:\_:\_:\_:\_:\_:\_:)

Creates a CFSocket object of a specified protocol and type.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFSocketCreate(
    _ allocator: CFAllocator!,
    _ protocolFamily: Int32,
    _ socketType: Int32,
    _ protocol: Int32,
    _ callBackTypes: CFOptionFlags,
    _ callout: CFSocketCallBack!,
    _ context: UnsafePointer!
) -> CFSocket!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`protocolFamily`  

The protocol family for the socket. If negative or 0 is passed, the socket defaults to `PF_INET`.

`socketType`  

The socket type to create. If `protocolFamily` is `PF_INET` and `socketType` is negative or 0, the socket type defaults to `SOCK_STREAM`.

`protocol`  

The protocol for the socket. If `protocolFamily` is `PF_INET` and `protocol` is negative or 0, the socket protocol defaults to `IPPROTO_TCP` if `socketType` is `SOCK_STREAM` or `IPPROTO_UDP` if `socketType` is `SOCK_DGRAM`.

`callBackTypes`  

A bitwise-OR combination of the types of socket activity that should cause `callout` to be called. See CFSocketCallBackType for the possible activity values.

`callout`  

The function to call when one of the activities indicated by `callBackTypes` occurs.

`context`  

A structure holding contextual information for the CFSocket object. The function copies the information out of the structure, so the memory pointed to by `context` does not need to persist beyond the function call. Can be `NULL`.

## Return Value

The new CFSocket object, or `NULL` if an error occurred. Ownership follows the The Create Rule.

## See Also

### Creating Sockets

func CFSocketCreateConnectedToSocketSignature(CFAllocator!, UnsafePointer&lt;CFSocketSignature>!, CFOptionFlags, CFSocketCallBack!, UnsafePointer&lt;CFSocketContext>!, CFTimeInterval) -> CFSocket!

Creates a CFSocket object and opens a connection to a remote socket.

func CFSocketCreateWithNative(CFAllocator!, CFSocketNativeHandle, CFOptionFlags, CFSocketCallBack!, UnsafePointer&lt;CFSocketContext>!) -> CFSocket!

Creates a CFSocket object for a pre-existing native socket.

func CFSocketCreateWithSocketSignature(CFAllocator!, UnsafePointer&lt;CFSocketSignature>!, CFOptionFlags, CFSocketCallBack!, UnsafePointer&lt;CFSocketContext>!) -> CFSocket!

Creates a CFSocket object using information from a CFSocketSignature structure.

