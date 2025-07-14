

- Core Foundation
-  CFRunLoopAddObserver(\_:\_:\_:) 

Function

# CFRunLoopAddObserver(\_:\_:\_:)

Adds a CFRunLoopObserver object to a run loop mode.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFRunLoopAddObserver(
    _ rl: CFRunLoop!,
    _ observer: CFRunLoopObserver!,
    _ mode: CFRunLoopMode!
)
```

## Parameters 

`rl`  

The run loop to modify.

`observer`  

The run loop observer to add.

`mode`  

The run loop mode to which to add `observer`. Use the constant commonModes to add `observer` to the set of objects monitored by all the common modes.

## Discussion

A run loop observer can be registered in only one run loop at a time, although it can be added to multiple run loop modes within that run loop.

If `rl` already contains `observer` in `mode`, this function does nothing.

## See Also

### Managing Observers

func CFRunLoopContainsObserver(CFRunLoop!, CFRunLoopObserver!, CFRunLoopMode!) -> Bool

Returns a Boolean value that indicates whether a run loop mode contains a particular CFRunLoopObserver object.

func CFRunLoopRemoveObserver(CFRunLoop!, CFRunLoopObserver!, CFRunLoopMode!)

Removes a CFRunLoopObserver object from a run loop mode.

