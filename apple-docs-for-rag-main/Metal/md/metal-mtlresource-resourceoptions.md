

- Metal
- MTLResource
-  resourceOptions 

Instance Property

# resourceOptions

The storage mode, CPU cache mode, and hazard tracking mode of the resource.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var resourceOptions: MTLResourceOptions { get }
```

**Required**

## Discussion

The value of this property aggregates the values of storageMode, cpuCacheMode, and hazardTrackingMode.

## See Also

### Reading Memory and Storage Properties

var cpuCacheMode: MTLCPUCacheMode

The CPU cache mode that defines the CPU mapping of the resource.

**Required**

var storageMode: MTLStorageMode

The location and access permissions of the resource.

**Required**

var hazardTrackingMode: MTLHazardTrackingMode

A mode that determines whether Metal tracks and synchronizes resource access.

**Required**

enum MTLCPUCacheMode

Options for the CPU cache mode that define the CPU mapping of the resource.

enum MTLStorageMode

Options for the memory location and access permissions for a resource.

enum MTLHazardTrackingMode

The options you use to specify the hazard tracking mode.

