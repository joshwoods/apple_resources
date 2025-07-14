

- Metal
- MTLHeap
-  storageMode 

Instance Property

# storageMode

The heap’s storage mode.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
var storageMode: MTLStorageMode { get }
```

**Required**

## Discussion

Any resources you allocate on the heap have this storage mode.

## See Also

### Querying Heap Properties

var type: MTLHeapType

The heap’s type.

**Required**

var cpuCacheMode: MTLCPUCacheMode

The heap’s CPU cache mode.

**Required**

var hazardTrackingMode: MTLHazardTrackingMode

The heap’s hazard tracking mode.

**Required**

var resourceOptions: MTLResourceOptions

The options for resources created by the heap.

**Required**

var size: Int

The total size of the heap, in bytes.

**Required**

var usedSize: Int

The size of all resources currently in the heap, in bytes.

**Required**

var currentAllocatedSize: Int

The size, in bytes, of the current heap allocation.

**Required**

func maxAvailableSize(alignment: Int) -> Int

The maximum size of a resource, in bytes, that can be currently allocated from the heap.

**Required**

enum MTLHeapType

The options you use to choose the heap type.

