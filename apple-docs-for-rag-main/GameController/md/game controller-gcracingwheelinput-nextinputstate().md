

- Game Controller
- GCRacingWheelInput
-  nextInputState() 

Instance Method

# nextInputState()

Returns the next input state of the racing wheel from the queue.

Mac Catalyst 16.0+macOS 13.0+

``` source
func nextInputState() -> (any GCRacingWheelInputState & GCDevicePhysicalInputStateDiff)?
```

## Return Value

The next input state in the queue or `nil` if the queue is empty.

## Discussion

This method removes the next input state from the queue.

