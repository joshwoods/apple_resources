

- Core Foundation
-  CFRunLoopAddSource(\_:\_:\_:) 

Function

# CFRunLoopAddSource(\_:\_:\_:)

Adds a CFRunLoopSource object to a run loop mode.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFRunLoopAddSource(
    _ rl: CFRunLoop!,
    _ source: CFRunLoopSource!,
    _ mode: CFRunLoopMode!
)
```

## Parameters 

`rl`  

The run loop to modify.

`source`  

The run loop source to add. The source is retained by the run loop.

`mode`  

The run loop mode to which to add `source`. Use the constant commonModes to add `source` to the set of objects monitored by all the common modes.

## Discussion

If `source` is a version 0 source, this function calls the `schedule` callback function specified in the context structure for `source`. See CFRunLoopSourceContext for more details.

A run loop source can be registered in multiple run loops and run loop modes at the same time. When the source is signaled, whichever run loop that happens to detect the signal first will fire the source.

If `rl` already contains `source` in `mode`, this function does nothing.

## See Also

### Managing Sources

func CFRunLoopContainsSource(CFRunLoop!, CFRunLoopSource!, CFRunLoopMode!) -> Bool

Returns a Boolean value that indicates whether a run loop mode contains a particular CFRunLoopSource object.

func CFRunLoopRemoveSource(CFRunLoop!, CFRunLoopSource!, CFRunLoopMode!)

Removes a CFRunLoopSource object from a run loop mode.

