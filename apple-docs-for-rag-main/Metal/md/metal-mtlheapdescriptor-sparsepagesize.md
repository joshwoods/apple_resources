

- Metal
- MTLHeapDescriptor
-  sparsePageSize 

Instance Property

# sparsePageSize

The page size for any resources you allocate from the heaps you create with this descriptor.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var sparsePageSize: MTLSparsePageSize { get set }
```

## Discussion

This property’s default value is 16 kilobytes (MTLSparsePageSize.size16), which is a smaller page size option that can help reduce your app’s memory usage. However, you can reduce operational overhead for sparse textures with larger page sizes, such as MTLSparsePageSize.size64 and MTLSparsePageSize.size256. These operations include blit commands and the configuration of sparse texture mappings (see Blit Passes and MTLResourceStateCommandEncoder, respectively).

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

var size: Int

The total amount of memory, in bytes, for the heaps you create with this descriptor.

