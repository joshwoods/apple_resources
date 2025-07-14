

- Game Controller
- GCDevicePhysicalInputStateDiff
-  changedElements() 

Instance Method

# changedElements()

Returns the elements that changed since the previous input state.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOS

``` source
func changedElements() -> (some Sequence)?
```

## Return Value

A sequence that contains the changed elements in no particular order.

## Mentioned in 

Handling input events

## Discussion

Returns `nil` if there’s no previous input state, either because this is the first input state or Game Controller discards the prior input state because the queue is full.

## See Also

### Getting changes

func change(for: any GCPhysicalInputElement) -> GCDevicePhysicalInputElementChange

Returns whether the input value of an element changes.

**Required**

enum GCDevicePhysicalInputElementChange

Possible values that describe whether the input value of an element changes.

func changedElements() -> NSEnumerator?

Returns the elements that changed since the previous input state.

