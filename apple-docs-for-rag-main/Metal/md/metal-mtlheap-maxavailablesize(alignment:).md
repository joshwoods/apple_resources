

- Metal
- MTLHeap
-  maxAvailableSize(alignment:) 

Instance Method

# maxAvailableSize(alignment:)

The maximum size of a resource, in bytes, that can be currently allocated from the heap.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
func maxAvailableSize(alignment: Int) -> Int
```

**Required**

## Parameters 

`alignment`  

The alignment of the resource, in bytes. This value must be a power of two.

## Return Value

The maximum size for the resource, in bytes.

## Discussion

This method measures fragmentation within the heap. You can use the heapBufferSizeAndAlign(length:options:) and heapTextureSizeAndAlign(descriptor:) methods to help you determine the correct alignment for the resource.

## See Also

### Querying Heap Properties

var type: MTLHeapType

The heap’s type.

**Required**

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

enum MTLHeapType

The options you use to choose the heap type.

