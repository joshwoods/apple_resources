

- Game Controller
-  GCDevicePhysicalInputElementChange 

Enumeration

# GCDevicePhysicalInputElementChange

Possible values that describe whether the input value of an element changes.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
enum GCDevicePhysicalInputElementChange
```

## Topics

### States

case unknownChange

It’s unknown whether there’s a change to the input value.

case noChange

There’s no change to the input value.

case changed

There’s a change to the input value.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting changes

func change(for: any GCPhysicalInputElement) -> GCDevicePhysicalInputElementChange

Returns whether the input value of an element changes.

**Required**

func changedElements() -> NSEnumerator?

Returns the elements that changed since the previous input state.

func changedElements() -> (some Sequence&lt;any GCPhysicalInputElement>)? 

Returns the elements that changed since the previous input state.

