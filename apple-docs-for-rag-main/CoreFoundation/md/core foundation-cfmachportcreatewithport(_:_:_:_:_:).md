

- Core Foundation
-  CFMachPortCreateWithPort(\_:\_:\_:\_:\_:) 

Function

# CFMachPortCreateWithPort(\_:\_:\_:\_:\_:)

Creates a CFMachPort object for a pre-existing native Mach port.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFMachPortCreateWithPort(
    _ allocator: CFAllocator!,
    _ portNum: mach_port_t,
    _ callout: CFMachPortCallBack!,
    _ context: UnsafeMutablePointer!,
    _ shouldFreeInfo: UnsafeMutablePointer!
) -> CFMachPort!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`portNum`  

The native Mach port to use.

`callout`  

The callback function invoked when a message is received on the Mach port.

`context`  

A structure holding contextual information for the Mach port. The function copies the information out of the structure, so the memory pointed to by `context` does not need to persist beyond the function call.

`shouldFreeInfo`  

A flag set by the function to indicate whether the `info` member of `context` should be freed. The flag is set to `true` on failure or if a CFMachPort object already exists for `portNum`, `false` otherwise. `shouldFreeInfo` can be `NULL`.

## Return Value

The new CFMachPort object or `NULL` on failure. If a CFMachPort object already exists for `portNum`, the function returns the pre-existing object instead of creating a new object; the `context` and `callout` parameters are ignored in this case. Ownership follows the The Create Rule.

## Discussion

The CFMachPort object does not take full ownership of the send and receive rights of the Mach port `portNum`. It is the caller’s responsibility to deallocate the Mach port rights after the CFMachPort object is no longer needed and has been invalidated.

## See Also

### Creating a CFMachPort Object

func CFMachPortCreate(CFAllocator!, CFMachPortCallBack!, UnsafeMutablePointer&lt;CFMachPortContext>!, UnsafeMutablePointer&lt;DarwinBoolean>!) -> CFMachPort!

Creates a CFMachPort object with a new Mach port.

