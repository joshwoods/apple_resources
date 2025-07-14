

- Metal
-  MTLStorageMode 

Enumeration

# MTLStorageMode

Options for the memory location and access permissions for a resource.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
enum MTLStorageMode
```

## Mentioned in 

Setting Resource Storage Modes

## Overview

For more guidance on how to choose storage modes, see Setting Resource Storage Modes.

## Topics

### Storage Mode Options

case shared

The CPU and GPU share access to the resource, allocated in system memory.

case managed

The CPU and GPU may maintain separate copies of the resource, and any changes must be explicitly synchronized.

case `private`

The resource is only available to the GPU.

case memoryless

The resource’s contents are only available to the GPU, and only exist temporarily during a render pass.

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

enum MTLHazardTrackingMode

The options you use to specify the hazard tracking mode.

