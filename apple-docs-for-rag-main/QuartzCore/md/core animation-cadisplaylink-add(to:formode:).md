

- Core Animation
- CADisplayLink
-  add(to:forMode:) 

Instance Method

# add(to:forMode:)

Registers the display link with a run loop.

iOS 3.1+iPadOS 3.1+Mac Catalyst 13.1+macOS 14.0+tvOS 9.0+visionOS 1.0+

``` source
func add(
    to runloop: RunLoop,
    forMode mode: RunLoop.Mode
)
```

## Parameters 

`runloop`  

The run loop to associate with the display link.

`mode`  

The mode in which to add the display link to the run loop.

## Discussion

You can associate a display link with multiple input modes. While the run loop is executing in a mode you specify, the display link notifies the target when the system requires new frames.

You can specify a custom mode or use one of the modes listed in RunLoop.

The run loop retains the display link. To remove the display link from all run loops, call invalidate().

## See Also

### Scheduling a Display Link to Send Notifications

func remove(from: RunLoop, forMode: RunLoop.Mode)

Removes the display link from the run loop for the given mode.

func invalidate()

Removes the display link from all run loop modes.

