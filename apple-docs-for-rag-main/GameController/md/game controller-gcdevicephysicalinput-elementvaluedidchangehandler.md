

- Game Controller
- GCDevicePhysicalInput
-  elementValueDidChangeHandler 

Instance Property

# elementValueDidChangeHandler

A block that the profile calls when an element’s value changes.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var elementValueDidChangeHandler: ((any GCDevicePhysicalInput, any GCPhysicalInputElement) -> Void)? { get set }
```

**Required**

## Mentioned in 

Handling input events

## Discussion

Use this property to get the latest state of the element. If multiple elements change, Game Controller invokes this block for each element that changes. The block’s parameters are:

element  
The element whose value changes.

Important

To track every element value change, set the inputStateAvailableHandler property instead and use the nextInputState() method to get all the buffered changes.

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

func capture() -> any GCDevicePhysicalInputState

Returns a snapshot of the physical device inputs.

**Required**

