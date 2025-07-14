

- Game Controller
- GCControllerLiveInput
-  capture() 

Instance Method

# capture()

Returns a snapshot of the physical device inputs.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
func capture() -> GCControllerInputState
```

## Return Value

A new instance containing the current state of the physical device input.

## See Also

### Handling device input

func nextInputState() -> (any GCControllerInputState &amp; GCDevicePhysicalInputStateDiff)?

Returns the next device input state from the queue.

