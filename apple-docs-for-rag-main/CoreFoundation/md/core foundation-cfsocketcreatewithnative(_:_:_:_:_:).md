

- Core Foundation
-  CFSocketCreateWithNative(\_:\_:\_:\_:\_:) 

Function

# CFSocketCreateWithNative(\_:\_:\_:\_:\_:)

Creates a CFSocket object for a pre-existing native socket.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFSocketCreateWithNative(
    _ allocator: CFAllocator!,
    _ sock: CFSocketNativeHandle,
    _ callBackTypes: CFOptionFlags,
    _ callout: CFSocketCallBack!,
    _ context: UnsafePointer!
) -> CFSocket!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`sock`  

The native socket for which to create a CFSocket object.

`callBackTypes`  

A bitwise-OR combination of the types of socket activity that should cause `callout` to be called. See CFSocketCallBackType for the possible activity values.

`callout`  

The function to call when one of the activities indicated by `callBackTypes` occurs.

`context`  

A structure holding contextual information for the CFSocket object. The function copies the information out of the structure, so the memory pointed to by `context` does not need to persist beyond the function call. Can be `NULL`.

## Return Value

The new CFSocket object, or `NULL` if an error occurred. If a CFSocket object already exists for `sock`, the function returns the pre-existing object instead of creating a new object; the `context`, `callout`, and `callBackTypes` parameters are ignored in this case. Ownership follows the The Create Rule.

## See Also

### Creating Sockets

func CFSocketCreate(CFAllocator!, Int32, Int32, Int32, CFOptionFlags, CFSocketCallBack!, UnsafePointer&lt;CFSocketContext>!) -> CFSocket!

Creates a CFSocket object of a specified protocol and type.

func CFSocketCreateConnectedToSocketSignature(CFAllocator!, UnsafePointer&lt;CFSocketSignature>!, CFOptionFlags, CFSocketCallBack!, UnsafePointer&lt;CFSocketContext>!, CFTimeInterval) -> CFSocket!

Creates a CFSocket object and opens a connection to a remote socket.

func CFSocketCreateWithSocketSignature(CFAllocator!, UnsafePointer&lt;CFSocketSignature>!, CFOptionFlags, CFSocketCallBack!, UnsafePointer&lt;CFSocketContext>!) -> CFSocket!

Creates a CFSocket object using information from a CFSocketSignature structure.

