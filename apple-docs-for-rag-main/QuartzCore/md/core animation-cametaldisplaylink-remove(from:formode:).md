

- Core Animation
- CAMetalDisplayLink
-  remove(from:forMode:) 

Instance Method

# remove(from:forMode:)

Removes a mode’s display link from a run loop.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
func remove(
    from runloop: RunLoop,
    forMode mode: RunLoop.Mode
)
```

## Parameters 

`runloop`  

A run loop the method disassociates the display link from for `mode`.

`mode`  

A run loop mode the method disassociates the display link for `runloop`.

## Discussion

The run loop releases the display link if it no longer associates with any run modes.

## See Also

### Deregistering for callbacks

func invalidate()

Removes the display link from all run loops for all modes.

