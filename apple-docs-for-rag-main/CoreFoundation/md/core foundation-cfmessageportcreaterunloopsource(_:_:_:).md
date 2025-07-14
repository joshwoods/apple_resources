

- Core Foundation
-  CFMessagePortCreateRunLoopSource(\_:\_:\_:) 

Function

# CFMessagePortCreateRunLoopSource(\_:\_:\_:)

Creates a CFRunLoopSource object for a CFMessagePort object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFMessagePortCreateRunLoopSource(
    _ allocator: CFAllocator!,
    _ local: CFMessagePort!,
    _ order: CFIndex
) -> CFRunLoopSource!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`local`  

The message port for which to create a run loop source.

`order`  

A priority index indicating the order in which run loop sources are processed. `order` is currently ignored by CFMessagePort object run loop sources. Pass `0` for this value.

## Return Value

The new CFRunLoopSource object for `ms`. Ownership follows the The Create Rule.

## Discussion

The run loop source is not automatically added to a run loop. To add the source to a run loop, use CFRunLoopAddSource(_:_:_:).

### Special Considerations

This method is not available on iOS 7 and later—it will return `NULL` and log a sandbox violation in `syslog`. See Concurrency Programming Guide for possible replacement technologies.

## See Also

### Configuring a CFMessagePort Object

func CFMessagePortSetInvalidationCallBack(CFMessagePort!, CFMessagePortInvalidationCallBack!)

Sets the callback function invoked when a CFMessagePort object is invalidated.

func CFMessagePortSetName(CFMessagePort!, CFString!) -> Bool

Sets the name of a local CFMessagePort object.

