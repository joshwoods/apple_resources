

- Core Foundation
-  CFMachPortCreateRunLoopSource(\_:\_:\_:) 

Function

# CFMachPortCreateRunLoopSource(\_:\_:\_:)

Creates a CFRunLoopSource object for a CFMachPort object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFMachPortCreateRunLoopSource(
    _ allocator: CFAllocator!,
    _ port: CFMachPort!,
    _ order: CFIndex
) -> CFRunLoopSource!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`port`  

The Mach port for which to create a CFRunLoopSource object.

`order`  

A priority index indicating the order in which run loop sources are processed. `order` is currently ignored by CFMachPort run loop sources. Pass `0` for this value.

## Return Value

The new CFRunLoopSource object for `port`. Ownership follows the The Create Rule.

## Discussion

The run loop source is not automatically added to a run loop. To add the source to a run loop, use CFRunLoopAddSource(_:_:_:).

## See Also

### Configuring a CFMachPort Object

func CFMachPortInvalidate(CFMachPort!)

Invalidates a CFMachPort object, stopping it from receiving any more messages.

func CFMachPortSetInvalidationCallBack(CFMachPort!, CFMachPortInvalidationCallBack!)

Sets the callback function invoked when a CFMachPort object is invalidated.

