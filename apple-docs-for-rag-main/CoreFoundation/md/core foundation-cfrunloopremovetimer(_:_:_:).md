

- Core Foundation
-  CFRunLoopRemoveTimer(\_:\_:\_:) 

Function

# CFRunLoopRemoveTimer(\_:\_:\_:)

Removes a CFRunLoopTimer object from a run loop mode.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFRunLoopRemoveTimer(
    _ rl: CFRunLoop!,
    _ timer: CFRunLoopTimer!,
    _ mode: CFRunLoopMode!
)
```

## Parameters 

`rl`  

The run loop to modify.

`timer`  

The run loop timer to remove.

`mode`  

The run loop mode of `rl` from which to remove `timer`. Use the constant commonModes to remove `timer` from the set of objects monitored by all the common modes.

## Discussion

If `rl` does not contain `timer` in `mode`, this function does nothing.

## See Also

### Managing Timers

func CFRunLoopAddTimer(CFRunLoop!, CFRunLoopTimer!, CFRunLoopMode!)

Adds a CFRunLoopTimer object to a run loop mode.

func CFRunLoopGetNextTimerFireDate(CFRunLoop!, CFRunLoopMode!) -> CFAbsoluteTime

Returns the time at which the next timer will fire.

func CFRunLoopContainsTimer(CFRunLoop!, CFRunLoopTimer!, CFRunLoopMode!) -> Bool

Returns a Boolean value that indicates whether a run loop mode contains a particular CFRunLoopTimer object.

