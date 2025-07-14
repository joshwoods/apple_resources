

- Core Foundation
-  CFRunLoopGetNextTimerFireDate(\_:\_:) 

Function

# CFRunLoopGetNextTimerFireDate(\_:\_:)

Returns the time at which the next timer will fire.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFRunLoopGetNextTimerFireDate(
    _ rl: CFRunLoop!,
    _ mode: CFRunLoopMode!
) -> CFAbsoluteTime
```

## Parameters 

`rl`  

The run loop to examine.

`mode`  

The run loop mode within `rl` to test.

## Return Value

The earliest firing time of the run loop timers registered in `mode` for the run loop `rl`.

## See Also

### Managing Timers

func CFRunLoopAddTimer(CFRunLoop!, CFRunLoopTimer!, CFRunLoopMode!)

Adds a CFRunLoopTimer object to a run loop mode.

func CFRunLoopRemoveTimer(CFRunLoop!, CFRunLoopTimer!, CFRunLoopMode!)

Removes a CFRunLoopTimer object from a run loop mode.

func CFRunLoopContainsTimer(CFRunLoop!, CFRunLoopTimer!, CFRunLoopMode!) -> Bool

Returns a Boolean value that indicates whether a run loop mode contains a particular CFRunLoopTimer object.

