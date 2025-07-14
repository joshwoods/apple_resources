

- System Configuration
-  SCDynamicStoreCreateRunLoopSource(\_:\_:\_:) 

Function

# SCDynamicStoreCreateRunLoopSource(\_:\_:\_:)

Creates a run loop source object that can be added to the application’s run loop.

macOS 10.1+

``` source
func SCDynamicStoreCreateRunLoopSource(
    _ allocator: CFAllocator?,
    _ store: SCDynamicStore,
    _ order: CFIndex
) -> CFRunLoopSource?
```

## Parameters 

`allocator`  

The allocator that should be used to allocate memory for the run loop source. This parameter may be `NULL` in which case the current default allocator is used. If this value is not a valid CFAllocator, the behavior is undefined.

`store`  

The dynamic store session.

`order`  

The order in which the sources that are ready to be processed are handled, on platforms that support it and for source versions that support it. A source with a lower order number is processed before a source with a higher order number. It is inadvisable to depend on the order number for any architectural or design aspect of code. In the absence of any reason to do otherwise, pass `0` for this parameter.

## Return Value

The new run loop source object. You must release the returned value.

## Discussion

Note that all dynamic store notifications are delivered using the run loop source this function returns.

