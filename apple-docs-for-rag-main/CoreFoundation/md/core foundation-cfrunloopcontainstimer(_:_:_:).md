

- Core Foundation
-  CFRunLoopContainsTimer(\_:\_:\_:) 

Function

# CFRunLoopContainsTimer(\_:\_:\_:)

Returns a Boolean value that indicates whether a run loop mode contains a particular CFRunLoopTimer object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFRunLoopContainsTimer(
    _ rl: CFRunLoop!,
    _ timer: CFRunLoopTimer!,
    _ mode: CFRunLoopMode!
) -> Bool
```

## Parameters 

`rl`  

The run loop to examine.

`timer`  

The run loop timer for which to search.

`mode`  

The run loop mode of `rl` in which to search for `timer`. Use the constant commonModes to search for `timer` in the set of objects monitored by all the common modes.

## Return Value

`true` if `timer` is in mode `mode` of the run loop `rl`, `false` otherwise.

## Discussion

If `timer` was added to commonModes, this function returns `true` if `mode` is either commonModes or any of the modes that has been added to the set of common modes.

## See Also

### Managing Timers

func CFRunLoopAddTimer(CFRunLoop!, CFRunLoopTimer!, CFRunLoopMode!)

Adds a CFRunLoopTimer object to a run loop mode.

func CFRunLoopGetNextTimerFireDate(CFRunLoop!, CFRunLoopMode!) -> CFAbsoluteTime

Returns the time at which the next timer will fire.

func CFRunLoopRemoveTimer(CFRunLoop!, CFRunLoopTimer!, CFRunLoopMode!)

Removes a CFRunLoopTimer object from a run loop mode.

