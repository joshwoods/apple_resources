

- Metal
-  MTLHazardTrackingMode 

Enumeration

# MTLHazardTrackingMode

The options you use to specify the hazard tracking mode.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
enum MTLHazardTrackingMode
```

## Topics

### Specifying the Tracking Mode

case `default`

An option specifying that the default tracking mode should be used.

case untracked

An option specifying that the app must prevent hazards when modifying this object’s contents.

case tracked

An option specifying that Metal prevents hazards when modifying this object’s contents.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

var resourceOptions: MTLResourceOptions

The storage mode, CPU cache mode, and hazard tracking mode of the resource.

**Required**

enum MTLCPUCacheMode

Options for the CPU cache mode that define the CPU mapping of the resource.

enum MTLStorageMode

Options for the memory location and access permissions for a resource.

