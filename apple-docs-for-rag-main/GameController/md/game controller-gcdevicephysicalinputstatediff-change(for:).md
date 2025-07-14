

- Game Controller
- GCDevicePhysicalInputStateDiff
-  change(for:) 

Instance Method

# change(for:)

Returns whether the input value of an element changes.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func change(for element: any GCPhysicalInputElement) -> GCDevicePhysicalInputElementChange
```

**Required**

## Parameters 

`element`  

The element whose value changes.

## Return Value

Description of the change to the element.

## Mentioned in 

Handling input events

## See Also

### Getting changes

enum GCDevicePhysicalInputElementChange

Possible values that describe whether the input value of an element changes.

func changedElements() -> NSEnumerator?

Returns the elements that changed since the previous input state.

func changedElements() -> (some Sequence&lt;any GCPhysicalInputElement>)? 

Returns the elements that changed since the previous input state.

