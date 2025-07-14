

- Game Controller
- GCDevicePhysicalInput
-  capture() 

Instance Method

# capture()

Returns a snapshot of the physical device inputs.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func capture() -> any GCDevicePhysicalInputState
```

**Required**

## Return Value

A new instance containing the current state of the physical device input.

## Mentioned in 

Handling input events

## See Also

### Handling device input

func nextInputState() -> (any GCDevicePhysicalInputState &amp; GCDevicePhysicalInputStateDiff)?

Returns the next input state from the queue.

**Required**

var inputStateAvailableHandler: ((any GCDevicePhysicalInput) -> Void)?

The block that the profile calls when Game Controller adds an input state to the queue.

**Required**

var inputStateQueueDepth: Int

The maximum number of input values that the queue stores.

**Required**

var elementValueDidChangeHandler: ((any GCDevicePhysicalInput, any GCPhysicalInputElement) -> Void)?

A block that the profile calls when an element’s value changes.

**Required**

