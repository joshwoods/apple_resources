

- Metal
- MTLPurgeableState
-  MTLPurgeableState.nonVolatile 

Case

# MTLPurgeableState.nonVolatile

The contents of the resource aren’t allowed to be discarded.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
case nonVolatile
```

## See Also

### Specifying Purgeable States

case keepCurrent

The current state is queried but doesn’t change.

case volatile

The system is allowed to discard the resource to free up memory.

case empty

A state that indicates to the system that it needs to consider the contents of a resource as invalid, typically because you’re discarding it.

