

- Metal
- MTLResource
-  hazardTrackingMode 

Instance Property

# hazardTrackingMode

A mode that determines whether Metal tracks and synchronizes resource access.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var hazardTrackingMode: MTLHazardTrackingMode { get }
```

**Required**

## Discussion

This value can be either MTLHazardTrackingMode.untracked or MTLHazardTrackingMode.tracked.

## See Also

### Reading Memory and Storage Properties

var cpuCacheMode: MTLCPUCacheMode

The CPU cache mode that defines the CPU mapping of the resource.

**Required**

var storageMode: MTLStorageMode

The location and access permissions of the resource.

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

