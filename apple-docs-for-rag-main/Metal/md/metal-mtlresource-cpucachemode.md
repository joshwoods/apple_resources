

- Metal
- MTLResource
-  cpuCacheMode 

Instance Property

# cpuCacheMode

The CPU cache mode that defines the CPU mapping of the resource.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var cpuCacheMode: MTLCPUCacheMode { get }
```

**Required**

## Discussion

The cache mode is set when you create the resource and cannot be changed.

## See Also

### Reading Memory and Storage Properties

var storageMode: MTLStorageMode

The location and access permissions of the resource.

**Required**

var hazardTrackingMode: MTLHazardTrackingMode

A mode that determines whether Metal tracks and synchronizes resource access.

**Required**

var resourceOptions: MTLResourceOptions

The storage mode, CPU cache mode, and hazard tracking mode of the resource.

**Required**

enum MTLCPUCacheMode

Options for the CPU cache mode that define the CPU mapping of the resource.

enum MTLStorageMode

Options for the memory location and access permissions for a resource.

enum MTLHazardTrackingMode

The options you use to specify the hazard tracking mode.

