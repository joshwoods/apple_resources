

- Metal
- MTLHeapDescriptor
-  type 

Instance Property

# type

The memory placement strategy for any resources you allocate from the heaps you create with this descriptor.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var type: MTLHeapType { get set }
```

## Discussion

This property’s default value is MTLHeapType.automatic.

## See Also

### Configuring a Heap

var storageMode: MTLStorageMode

The storage mode for the heaps you create with this descriptor.

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

