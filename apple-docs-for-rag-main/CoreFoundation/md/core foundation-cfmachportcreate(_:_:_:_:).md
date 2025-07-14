

- Core Foundation
-  CFMachPortCreate(\_:\_:\_:\_:) 

Function

# CFMachPortCreate(\_:\_:\_:\_:)

Creates a CFMachPort object with a new Mach port.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFMachPortCreate(
    _ allocator: CFAllocator!,
    _ callout: CFMachPortCallBack!,
    _ context: UnsafeMutablePointer!,
    _ shouldFreeInfo: UnsafeMutablePointer!
) -> CFMachPort!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`callout`  

The callback function invoked when a message is received on the new Mach port.

`context`  

A structure holding contextual information for the new Mach port. The function copies the information out of the structure, so the memory pointed to by `context` does not need to persist beyond the function call.

`shouldFreeInfo`  

A flag set by the function to indicate whether the `info` member of `context` should be freed. The flag is set to `true` on failure, `false` otherwise. `shouldFreeInfo` can be `NULL`.

## Return Value

The new CFMachPort object or `NULL` on failure. The CFMachPort object has both send and receive rights. Ownership follows the The Create Rule.

## See Also

### Creating a CFMachPort Object

func CFMachPortCreateWithPort(CFAllocator!, mach_port_t, CFMachPortCallBack!, UnsafeMutablePointer&lt;CFMachPortContext>!, UnsafeMutablePointer&lt;DarwinBoolean>!) -> CFMachPort!

Creates a CFMachPort object for a pre-existing native Mach port.

