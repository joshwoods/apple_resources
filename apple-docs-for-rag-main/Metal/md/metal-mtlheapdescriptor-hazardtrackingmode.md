

- Metal
- MTLHeapDescriptor
-  hazardTrackingMode 

Instance Property

# hazardTrackingMode

The hazard tracking behavior for any resources you allocate from the heaps you create with this descriptor.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var hazardTrackingMode: MTLHazardTrackingMode { get set }
```

## Discussion

This property’s default value is MTLHazardTrackingMode.default, which is equivalent to MTLHazardTrackingMode.untracked for a heap.

The resources you allocate from a heap inherit that heap’s hazard tracking mode.

## See Also

### Configuring a Heap

var type: MTLHeapType

The memory placement strategy for any resources you allocate from the heaps you create with this descriptor.

var storageMode: MTLStorageMode

The storage mode for the heaps you create with this descriptor.

var cpuCacheMode: MTLCPUCacheMode

The CPU cache behavior for any resources you allocate from the heaps you create with this descriptor.

var resourceOptions: MTLResourceOptions

The combined behavior for any resources you allocate from the heaps you create with this descriptor.

var size: Int

The total amount of memory, in bytes, for the heaps you create with this descriptor.

var sparsePageSize: MTLSparsePageSize

The page size for any resources you allocate from the heaps you create with this descriptor.

