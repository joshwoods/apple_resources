

- Core Animation
- CADisplayLink
-  remove(from:forMode:) 

Instance Method

# remove(from:forMode:)

Removes the display link from the run loop for the given mode.

iOS 3.1+iPadOS 3.1+Mac Catalyst 13.1+macOS 14.0+tvOS 9.0+visionOS 1.0+

``` source
func remove(
    from runloop: RunLoop,
    forMode mode: RunLoop.Mode
)
```

## Parameters 

`runloop`  

The run loop you associate with the display link.

`mode`  

The run loop mode in which the display link is running.

## Discussion

The run loop releases the display link if it’s no longer associated with any run modes.

## See Also

### Scheduling a Display Link to Send Notifications

func add(to: RunLoop, forMode: RunLoop.Mode)

Registers the display link with a run loop.

func invalidate()

Removes the display link from all run loop modes.

