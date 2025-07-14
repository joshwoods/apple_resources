

- Core Foundation
-  CFRunLoopRemoveSource(\_:\_:\_:) 

Function

# CFRunLoopRemoveSource(\_:\_:\_:)

Removes a CFRunLoopSource object from a run loop mode.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFRunLoopRemoveSource(
    _ rl: CFRunLoop!,
    _ source: CFRunLoopSource!,
    _ mode: CFRunLoopMode!
)
```

## Parameters 

`rl`  

The run loop to modify.

`source`  

The run loop source to remove.

`mode`  

The run loop mode of `rl` from which to remove `source`. Use the constant commonModes to remove `source` from the set of objects monitored by all the common modes.

## Discussion

If `source` is a version 0 source, this function calls the `cancel` callback function specified in the context structure for `source`. See CFRunLoopSourceContext and CFRunLoopSourceContext1for more details.

If `rl` does not contain `source` in `mode`, this function does nothing.

## See Also

### Managing Sources

func CFRunLoopAddSource(CFRunLoop!, CFRunLoopSource!, CFRunLoopMode!)

Adds a CFRunLoopSource object to a run loop mode.

func CFRunLoopContainsSource(CFRunLoop!, CFRunLoopSource!, CFRunLoopMode!) -> Bool

Returns a Boolean value that indicates whether a run loop mode contains a particular CFRunLoopSource object.

