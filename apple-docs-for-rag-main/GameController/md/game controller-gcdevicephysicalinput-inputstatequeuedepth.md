

- Game Controller
- GCDevicePhysicalInput
-  inputStateQueueDepth 

Instance Property

# inputStateQueueDepth

The maximum number of input values that the queue stores.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var inputStateQueueDepth: Int { get set }
```

**Required**

## Discussion

When the queue reaches this limit, Game Controller starts removing the oldest input states from the queue. The default value for this property is `1` which indicates no buffering.

## See Also

### Handling device input

func nextInputState() -> (any GCDevicePhysicalInputState &amp; GCDevicePhysicalInputStateDiff)?

Returns the next input state from the queue.

**Required**

var inputStateAvailableHandler: ((any GCDevicePhysicalInput) -> Void)?

The block that the profile calls when Game Controller adds an input state to the queue.

**Required**

func capture() -> any GCDevicePhysicalInputState

Returns a snapshot of the physical device inputs.

**Required**

var elementValueDidChangeHandler: ((any GCDevicePhysicalInput, any GCPhysicalInputElement) -> Void)?

A block that the profile calls when an element’s value changes.

**Required**

