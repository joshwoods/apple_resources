

- Core Foundation
-  CFMessagePortCreateRemote(\_:\_:) 

Function

# CFMessagePortCreateRemote(\_:\_:)

Returns a CFMessagePort object connected to a remote port.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFMessagePortCreateRemote(
    _ allocator: CFAllocator!,
    _ name: CFString!
) -> CFMessagePort!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`name`  

The name of the remote message port to which to connect.

## Return Value

The new CFMessagePort object, or `NULL` on failure. If a message port has already been created for the remote port, the pre-existing object is returned. Ownership follows the The Create Rule.

## Discussion

This method is not available on iOS 7 and later—it will return `NULL` and log a sandbox violation in `syslog`. See Concurrency Programming Guide for possible replacement technologies.

## See Also

### Creating a CFMessagePort Object

func CFMessagePortCreateLocal(CFAllocator!, CFString!, CFMessagePortCallBack!, UnsafeMutablePointer&lt;CFMessagePortContext>!, UnsafeMutablePointer&lt;DarwinBoolean>!) -> CFMessagePort!

Returns a local CFMessagePort object.

