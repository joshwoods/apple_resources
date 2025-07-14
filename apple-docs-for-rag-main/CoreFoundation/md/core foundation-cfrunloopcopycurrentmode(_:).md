

- Core Foundation
-  CFRunLoopCopyCurrentMode(\_:) 

Function

# CFRunLoopCopyCurrentMode(\_:)

Returns the name of the mode in which a given run loop is currently running.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFRunLoopCopyCurrentMode(_ rl: CFRunLoop!) -> CFRunLoopMode!
```

## Parameters 

`rl`  

The run loop to examine.

## Return Value

The mode in which `rl` is currently running; `NULL` if `rl` is not running. Ownership follows the The Create Rule.

## Discussion

When run on the current thread’s run loop, the returned value identifies the run loop mode that made the callout in which your code is currently executing.

## See Also

### Managing Run Loop Modes

func CFRunLoopAddCommonMode(CFRunLoop!, CFRunLoopMode!)

Adds a mode to the set of run loop common modes.

func CFRunLoopCopyAllModes(CFRunLoop!) -> CFArray!

Returns an array that contains all the defined modes for a CFRunLoop object.

