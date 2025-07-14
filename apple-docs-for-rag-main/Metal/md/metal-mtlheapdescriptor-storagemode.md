

- Metal
- MTLHeapDescriptor
-  storageMode 

Instance Property

# storageMode

The storage mode for the heaps you create with this descriptor.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
var storageMode: MTLStorageMode { get set }
```

## Discussion

For devices with Apple silicon, you can create a heap with either the MTLStorageMode.private or the MTLStorageMode.shared storage mode. However, you can only create heaps with private storage on macOS devices without Apple silicon.

The resources you allocate from a heap inherit that heap’s storage mode. This property’s default value is MTLStorageMode.private.

## See Also

### Configuring a Heap

var type: MTLHeapType

The memory placement strategy for any resources you allocate from the heaps you create with this descriptor.

var cpuCacheMode: MTLCPUCacheMode

The CPU cache behavior for any resources you allocate from the heaps you create with this descriptor.

var hazardTrackingMode: MTLHazardTrackingMode

The hazard tracking behavior for any resources you allocate from the heaps you create with this descriptor.

var resourceOptions: MTLResourceOptions

The combined behavior for any resources you allocate from the heaps you create with this descriptor.

var size: Int

The total amount of memory, in bytes, for the heaps you create with this descriptor.

var sparsePageSize: MTLSparsePageSize

The page size for any resources you allocate from the heaps you create with this descriptor.

