

- Core Foundation
-  CFRunLoopCopyAllModes(\_:) 

Function

# CFRunLoopCopyAllModes(\_:)

Returns an array that contains all the defined modes for a CFRunLoop object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFRunLoopCopyAllModes(_ rl: CFRunLoop!) -> CFArray!
```

## Parameters 

`rl`  

The run loop to examine.

## Return Value

An array that contains all the run loop modes defined for `rl`. Ownership follows the The Create Rule.

## See Also

### Managing Run Loop Modes

func CFRunLoopAddCommonMode(CFRunLoop!, CFRunLoopMode!)

Adds a mode to the set of run loop common modes.

func CFRunLoopCopyCurrentMode(CFRunLoop!) -> CFRunLoopMode!

Returns the name of the mode in which a given run loop is currently running.

