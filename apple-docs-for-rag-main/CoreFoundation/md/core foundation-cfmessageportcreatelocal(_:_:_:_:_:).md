

- Core Foundation
-  CFMessagePortCreateLocal(\_:\_:\_:\_:\_:) 

Function

# CFMessagePortCreateLocal(\_:\_:\_:\_:\_:)

Returns a local CFMessagePort object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFMessagePortCreateLocal(
    _ allocator: CFAllocator!,
    _ name: CFString!,
    _ callout: CFMessagePortCallBack!,
    _ context: UnsafeMutablePointer!,
    _ shouldFreeInfo: UnsafeMutablePointer!
) -> CFMessagePort!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`name`  

The name with which to register the port. `name` can be `NULL`.

`callout`  

The callback function invoked when a message is received on the message port.

`context`  

A structure holding contextual information for the message port. The function copies the information out of the structure, so the memory pointed to by `context` does not need to persist beyond the function call.

`shouldFreeInfo`  

A flag set by the function to indicate whether the `info` member of `context` should be freed. The flag is set to `true` on failure or if a local port named `name` already exists, `false` otherwise. `shouldFreeInfo` can be `NULL`.

## Return Value

The new CFMessagePort object, or `NULL` on failure. If a local port is already named `name`, the function returns that port instead of creating a new object; the `context` and `callout` parameters are ignored in this case. Ownership follows the The Create Rule.

## Discussion

This method is not available on iOS 7 and later—it will return `NULL` and log a sandbox violation in `syslog`. See Concurrency Programming Guide for possible replacement technologies.

## See Also

### Creating a CFMessagePort Object

func CFMessagePortCreateRemote(CFAllocator!, CFString!) -> CFMessagePort!

Returns a CFMessagePort object connected to a remote port.

