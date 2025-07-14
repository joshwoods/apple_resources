

- Core Foundation
-  CFRunLoopContainsObserver(\_:\_:\_:) 

Function

# CFRunLoopContainsObserver(\_:\_:\_:)

Returns a Boolean value that indicates whether a run loop mode contains a particular CFRunLoopObserver object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFRunLoopContainsObserver(
    _ rl: CFRunLoop!,
    _ observer: CFRunLoopObserver!,
    _ mode: CFRunLoopMode!
) -> Bool
```

## Parameters 

`rl`  

The run loop to examine.

`observer`  

The run loop observer for which to search.

`mode`  

The run loop mode in which to search for `observer`. Use the constant commonModes to search for `observer` in the set of objects monitored by all the common modes.

## Return Value

`true` if `observer` is in mode `mode` of the run loop `rl`, otherwise `false`.

## Discussion

If `observer` was added to commonModes, this function returns `true` if `mode` is either commonModes or any of the modes that has been added to the set of common modes.

## See Also

### Managing Observers

func CFRunLoopAddObserver(CFRunLoop!, CFRunLoopObserver!, CFRunLoopMode!)

Adds a CFRunLoopObserver object to a run loop mode.

func CFRunLoopRemoveObserver(CFRunLoop!, CFRunLoopObserver!, CFRunLoopMode!)

Removes a CFRunLoopObserver object from a run loop mode.

