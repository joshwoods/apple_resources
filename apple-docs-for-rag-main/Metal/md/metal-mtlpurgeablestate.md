

- Metal
-  MTLPurgeableState 

Enumeration

# MTLPurgeableState

The purgeable state of the resource.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
enum MTLPurgeableState
```

## Topics

### Specifying Purgeable States

case keepCurrent

The current state is queried but doesn’t change.

case nonVolatile

The contents of the resource aren’t allowed to be discarded.

case volatile

The system is allowed to discard the resource to free up memory.

case empty

A state that indicates to the system that it needs to consider the contents of a resource as invalid, typically because you’re discarding it.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Setting the Purgeable State of the Resource

func setPurgeableState(MTLPurgeableState) -> MTLPurgeableState

Specifies or queries the resource’s purgeable state.

**Required**

