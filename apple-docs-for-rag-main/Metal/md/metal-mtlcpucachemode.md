

- Metal
-  MTLCPUCacheMode 

Enumeration

# MTLCPUCacheMode

Options for the CPU cache mode that define the CPU mapping of the resource.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
enum MTLCPUCacheMode
```

## Topics

### Specifying the Cache Mode

case defaultCache

The default CPU cache mode for the resource, which guarantees that read and write operations are executed in the expected order.

case writeCombined

A write-combined CPU cache mode that is optimized for resources that the CPU writes into, but never reads.

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

enum MTLStorageMode

Options for the memory location and access permissions for a resource.

enum MTLHazardTrackingMode

The options you use to specify the hazard tracking mode.

