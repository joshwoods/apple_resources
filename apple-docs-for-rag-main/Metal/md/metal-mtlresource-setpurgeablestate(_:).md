

- Metal
- MTLResource
-  setPurgeableState(\_:) 

Instance Method

# setPurgeableState(\_:)

Specifies or queries the resource’s purgeable state.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func setPurgeableState(_ state: MTLPurgeableState) -> MTLPurgeableState
```

**Required**

## Parameters 

`state`  

The desired purgeable state of a resource.

## Return Value

The prior purgeable state of the resource.

## Mentioned in 

Reducing the Memory Footprint of Metal Apps

## Discussion

If `state` is MTLPurgeableState.keepCurrent, the method returns the current purgeable state without changing it.

If `state` is MTLPurgeableState.nonVolatile, the resource is marked to inform the caller that the data should not be discarded.

If `state` is MTLPurgeableState.empty, the resource is marked as data that can be discarded, because the caller no longer needs the contents of the resource.

If `state` is MTLPurgeableState.volatile, the resource is marked as data that can be discarded, even if the caller may need the resource. `MTLResource` objects can be made purgeable, even if the caller may need the resource, where the implementation can reclaim the underlying storage at any time without informing the app. Purgeable resources may enable an app to keep larger caches of idle memory that may be useful again in the future without the risk of preventing the allocation of more important memory.

When you use purgeable memory, make sure the block of memory is locked before you access it. This locking mechanism is necessary to ensure that auto-removal policies do not discard the data while you are accessing it. Similarly, the locking mechanism ensures that the virtual memory system has not already discarded the data.

## See Also

### Setting the Purgeable State of the Resource

enum MTLPurgeableState

The purgeable state of the resource.

