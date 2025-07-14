

- Metal
- MTLHeap
-  setPurgeableState(\_:) 

Instance Method

# setPurgeableState(\_:)

Sets the purgeable state of the heap.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
func setPurgeableState(_ state: MTLPurgeableState) -> MTLPurgeableState
```

**Required**

## Parameters 

`state`  

The desired purgeable state of the heap.

## Return Value

The previous purgeable state of the heap.

## Discussion

The heap purgeability state refers to its whole backing memory and affects all resources in the heap. Heaps can be marked purgeable but its resources cannot; the heap’s resources always reflect the heap’s purgeability state.

Refer to the MTLPurgeableState and setPurgeableState(_:) reference for further information.

