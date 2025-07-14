

- Metal
- MTLHeap
-  type 

Instance Property

# type

The heap’s type.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var type: MTLHeapType { get }
```

**Required**

## See Also

### Querying Heap Properties

var storageMode: MTLStorageMode

The heap’s storage mode.

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

