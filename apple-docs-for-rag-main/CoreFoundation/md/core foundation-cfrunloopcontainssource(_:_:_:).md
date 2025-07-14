

- Core Foundation
-  CFRunLoopContainsSource(\_:\_:\_:) 

Function

# CFRunLoopContainsSource(\_:\_:\_:)

Returns a Boolean value that indicates whether a run loop mode contains a particular CFRunLoopSource object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFRunLoopContainsSource(
    _ rl: CFRunLoop!,
    _ source: CFRunLoopSource!,
    _ mode: CFRunLoopMode!
) -> Bool
```

## Parameters 

`rl`  

The run loop to examine.

`source`  

The run loop source for which to search.

`mode`  

The run loop mode of `rl` in which to search. Use the constant commonModes to search for `source` in the set of objects monitored by all the common modes.

## Return Value

`true` if `source` is in mode `mode` of the run loop `rl`, otherwise `false`.

## Discussion

If `source` was added to commonModes, this function returns `true` if `mode` is either commonModes or any of the modes that has been added to the set of common modes.

## See Also

### Managing Sources

func CFRunLoopAddSource(CFRunLoop!, CFRunLoopSource!, CFRunLoopMode!)

Adds a CFRunLoopSource object to a run loop mode.

func CFRunLoopRemoveSource(CFRunLoop!, CFRunLoopSource!, CFRunLoopMode!)

Removes a CFRunLoopSource object from a run loop mode.

