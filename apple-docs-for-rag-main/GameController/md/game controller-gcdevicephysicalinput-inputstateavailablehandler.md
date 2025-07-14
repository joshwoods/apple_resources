

- Game Controller
- GCDevicePhysicalInput
-  inputStateAvailableHandler 

Instance Property

# inputStateAvailableHandler

The block that the profile calls when Game Controller adds an input state to the queue.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var inputStateAvailableHandler: ((any GCDevicePhysicalInput) -> Void)? { get set }
```

**Required**

## Mentioned in 

Handling input events

## Discussion

Set this property to track every element value change, not just the current value. When Game Controller invokes the handler, invoke the nextInputState() method repeatedly to get all the buffered changes until the queue is empty.

To get just the current element value, use the elementValueDidChangeHandler property instead.

## See Also

### Handling device input

func nextInputState() -> (any GCDevicePhysicalInputState &amp; GCDevicePhysicalInputStateDiff)?

Returns the next input state from the queue.

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

