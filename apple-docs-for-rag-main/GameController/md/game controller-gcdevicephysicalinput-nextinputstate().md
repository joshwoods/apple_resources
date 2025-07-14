

- Game Controller
- GCDevicePhysicalInput
-  nextInputState() 

Instance Method

# nextInputState()

Returns the next input state from the queue.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func nextInputState() -> (any GCDevicePhysicalInputState & GCDevicePhysicalInputStateDiff)?
```

**Required**

## Return Value

The next input state in the queue or `nil` if the queue is empty.

## Mentioned in 

Handling input events

## Discussion

This method removes the next input state from the queue.

## See Also

### Handling device input

var inputStateAvailableHandler: ((any GCDevicePhysicalInput) -> Void)?

The block that the profile calls when Game Controller adds an input state to the queue.

**Required**

var inputStateQueueDepth: Int

The maximum number of input values that the queue stores.

**Required**

func capture() -> any GCDevicePhysicalInputState

Returns a snapshot of the physical device inputs.

**Required**

var elementValueDidChangeHandler: ((any GCDevicePhysicalInput, any GCPhysicalInputElement) -> Void)?

A block that the profile calls when an element’s value changes.

**Required**

