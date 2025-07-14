

- Core Foundation
-  CFSocketCreateConnectedToSocketSignature(\_:\_:\_:\_:\_:\_:) 

Function

# CFSocketCreateConnectedToSocketSignature(\_:\_:\_:\_:\_:\_:)

Creates a CFSocket object and opens a connection to a remote socket.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFSocketCreateConnectedToSocketSignature(
    _ allocator: CFAllocator!,
    _ signature: UnsafePointer!,
    _ callBackTypes: CFOptionFlags,
    _ callout: CFSocketCallBack!,
    _ context: UnsafePointer!,
    _ timeout: CFTimeInterval
) -> CFSocket!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`signature`  

A CFSocketSignature identifying the communication protocol and address to which the CFSocket object should connect.

`callBackTypes`  

A bitwise-OR combination of the types of socket activity that should cause `callout` to be called. See CFSocketCallBackType for the possible activity values.

`callout`  

The function to call when one of the activities indicated by `callBackTypes` occurs.

`context`  

A structure holding contextual information for the CFSocket object. The function copies the information out of the structure, so the memory pointed to by `context` does not need to persist beyond the function call. Can be `NULL`.

`timeout`  

The time to wait for a connection to succeed. If a negative value is used, this function does not wait for the connection and instead lets the connection attempt happen in the background. If `callBackTypes` includes `kCFSocketConnectCallBack`, you will receive a callback when the background connection succeeds or fails.

## Return Value

The new CFSocket object, or `NULL` if an error occurred. Ownership follows the The Create Rule.

## See Also

### Creating Sockets

func CFSocketCreate(CFAllocator!, Int32, Int32, Int32, CFOptionFlags, CFSocketCallBack!, UnsafePointer&lt;CFSocketContext>!) -> CFSocket!

Creates a CFSocket object of a specified protocol and type.

func CFSocketCreateWithNative(CFAllocator!, CFSocketNativeHandle, CFOptionFlags, CFSocketCallBack!, UnsafePointer&lt;CFSocketContext>!) -> CFSocket!

Creates a CFSocket object for a pre-existing native socket.

func CFSocketCreateWithSocketSignature(CFAllocator!, UnsafePointer&lt;CFSocketSignature>!, CFOptionFlags, CFSocketCallBack!, UnsafePointer&lt;CFSocketContext>!) -> CFSocket!

Creates a CFSocket object using information from a CFSocketSignature structure.

