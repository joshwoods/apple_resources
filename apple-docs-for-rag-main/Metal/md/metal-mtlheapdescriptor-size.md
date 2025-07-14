

- Metal
- MTLHeapDescriptor
-  size 

Instance Property

# size

The total amount of memory, in bytes, for the heaps you create with this descriptor.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
var size: Int { get set }
```

## Discussion

You can use various MTLDevice methods to help you estimate an appropriate heap size, including the following:

- heapBufferSizeAndAlign(length:options:)

- heapTextureSizeAndAlign(descriptor:)

- heapAccelerationStructureSizeAndAlign(size:)

- heapAccelerationStructureSizeAndAlign(descriptor:)

Note

Metal may round a heap’s size to a page boundary.

This property’s default value is `0`.

## See Also

### Configuring a Heap

var type: MTLHeapType

The memory placement strategy for any resources you allocate from the heaps you create with this descriptor.

var storageMode: MTLStorageMode

The storage mode for the heaps you create with this descriptor.

var cpuCacheMode: MTLCPUCacheMode

The CPU cache behavior for any resources you allocate from the heaps you create with this descriptor.

var hazardTrackingMode: MTLHazardTrackingMode

The hazard tracking behavior for any resources you allocate from the heaps you create with this descriptor.

var resourceOptions: MTLResourceOptions

The combined behavior for any resources you allocate from the heaps you create with this descriptor.

var sparsePageSize: MTLSparsePageSize

The page size for any resources you allocate from the heaps you create with this descriptor.

