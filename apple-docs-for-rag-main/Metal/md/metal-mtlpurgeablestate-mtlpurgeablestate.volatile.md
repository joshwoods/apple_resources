

- Metal
- MTLPurgeableState
-  MTLPurgeableState.volatile 

Case

# MTLPurgeableState.volatile

The system is allowed to discard the resource to free up memory.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
case volatile
```

## Mentioned in 

Reducing the Memory Footprint of Metal Apps

## See Also

### Specifying Purgeable States

case keepCurrent

The current state is queried but doesn’t change.

case nonVolatile

The contents of the resource aren’t allowed to be discarded.

case empty

A state that indicates to the system that it needs to consider the contents of a resource as invalid, typically because you’re discarding it.

