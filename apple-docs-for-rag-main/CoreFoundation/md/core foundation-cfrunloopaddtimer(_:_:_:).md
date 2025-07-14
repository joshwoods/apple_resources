

- Core Foundation
-  CFRunLoopAddTimer(\_:\_:\_:) 

Function

# CFRunLoopAddTimer(\_:\_:\_:)

Adds a CFRunLoopTimer object to a run loop mode.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFRunLoopAddTimer(
    _ rl: CFRunLoop!,
    _ timer: CFRunLoopTimer!,
    _ mode: CFRunLoopMode!
)
```

## Parameters 

`rl`  

The run loop to modify.

`timer`  

The run loop timer to add.

`mode`  

The run loop mode of `rl` to which to add `timer`. Use the constant commonModes to add `timer` to the set of objects monitored by all the common modes.

## Discussion

A run loop timer can be registered in only one run loop at a time, although it can be added to multiple run loop modes within that run loop.

If `rl` already contains `timer` in `mode`, this function does nothing.

## See Also

### Managing Timers

func CFRunLoopGetNextTimerFireDate(CFRunLoop!, CFRunLoopMode!) -> CFAbsoluteTime

Returns the time at which the next timer will fire.

func CFRunLoopRemoveTimer(CFRunLoop!, CFRunLoopTimer!, CFRunLoopMode!)

Removes a CFRunLoopTimer object from a run loop mode.

func CFRunLoopContainsTimer(CFRunLoop!, CFRunLoopTimer!, CFRunLoopMode!) -> Bool

Returns a Boolean value that indicates whether a run loop mode contains a particular CFRunLoopTimer object.

