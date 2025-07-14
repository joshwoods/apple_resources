

- Game Controller
- GCControllerLiveInput
-  nextInputState() 

Instance Method

# nextInputState()

Returns the next device input state from the queue.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
func nextInputState() -> (any GCControllerInputState & GCDevicePhysicalInputStateDiff)?
```

## Return Value

The next input state in the queue or `nil` if the queue is empty.

## See Also

### Handling device input

func capture() -> GCControllerInputState

Returns a snapshot of the physical device inputs.

