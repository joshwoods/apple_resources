

- Metal
- MTLPurgeableState
-  MTLPurgeableState.keepCurrent 

Case

# MTLPurgeableState.keepCurrent

The current state is queried but doesn’t change.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
case keepCurrent
```

## Discussion

The setPurgeableState(_:) method never returns this value. When this value is passed to that function, it returns the current purgability state without changing it.

## See Also

### Specifying Purgeable States

case nonVolatile

The contents of the resource aren’t allowed to be discarded.

case volatile

The system is allowed to discard the resource to free up memory.

case empty

A state that indicates to the system that it needs to consider the contents of a resource as invalid, typically because you’re discarding it.

