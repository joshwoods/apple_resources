

- Core Animation
- CADisplayLink
-  invalidate() 

Instance Method

# invalidate()

Removes the display link from all run loop modes.

iOS 3.1+iPadOS 3.1+Mac Catalyst 13.1+macOS 14.0+tvOS 9.0+visionOS 1.0+

``` source
func invalidate()
```

## Discussion

When you remove the display link from all run loop mode, the system releases it. The display link also releases the target.

This method is thread safe, so you can call it from a thread separate to the one in which the display link runs.

## See Also

### Scheduling a Display Link to Send Notifications

func add(to: RunLoop, forMode: RunLoop.Mode)

Registers the display link with a run loop.

func remove(from: RunLoop, forMode: RunLoop.Mode)

Removes the display link from the run loop for the given mode.

