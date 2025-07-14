

- Core Foundation
-  CFRunLoopRemoveObserver(\_:\_:\_:) 

Function

# CFRunLoopRemoveObserver(\_:\_:\_:)

Removes a CFRunLoopObserver object from a run loop mode.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFRunLoopRemoveObserver(
    _ rl: CFRunLoop!,
    _ observer: CFRunLoopObserver!,
    _ mode: CFRunLoopMode!
)
```

## Parameters 

`rl`  

The run loop to modify.

`observer`  

The run loop observer to remove.

`mode`  

The run loop mode of `rl` from which to remove `observer`. Use the constant commonModes to remove `observer` from the set of objects monitored by all the common modes.

## Discussion

If `rl` does not contain `observer` in `mode`, this function does nothing.

## See Also

### Managing Observers

func CFRunLoopAddObserver(CFRunLoop!, CFRunLoopObserver!, CFRunLoopMode!)

Adds a CFRunLoopObserver object to a run loop mode.

func CFRunLoopContainsObserver(CFRunLoop!, CFRunLoopObserver!, CFRunLoopMode!) -> Bool

Returns a Boolean value that indicates whether a run loop mode contains a particular CFRunLoopObserver object.

