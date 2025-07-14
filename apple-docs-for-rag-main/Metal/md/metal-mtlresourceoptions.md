

- Metal
-  MTLResourceOptions 

Structure

# MTLResourceOptions

Optional arguments used to set the behavior of a resource.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
struct MTLResourceOptions
```

## Mentioned in 

Setting Resource Storage Modes

## Topics

### Initializing Resource Options

init(rawValue: UInt)

### Specifying CPU Cache Modes

static var cpuCacheModeWriteCombined: MTLResourceOptions

A write-combined CPU cache mode that is optimized for resources that the CPU writes into, but never reads.

### Specifying Storage Modes

static var storageModeShared: MTLResourceOptions

The CPU and GPU share access to the resource, allocated in system memory.

static var storageModeManaged: MTLResourceOptions

The CPU and GPU may maintain separate copies of the resource, and any changes must be explicitly synchronized.

static var storageModePrivate: MTLResourceOptions

The resource is only available to the GPU.

static var storageModeMemoryless: MTLResourceOptions

The resource’s contents are only available to the GPU, and only exist temporarily during a render pass.

### Specifying Hazard Tracking

static var hazardTrackingModeTracked: MTLResourceOptions

An option specifying that Metal prevents hazards when modifying this object’s contents.

static var hazardTrackingModeUntracked: MTLResourceOptions

An option specifying that the app must prevent hazards when modifying this object’s contents.

### Deprecated Options

static var optionCPUCacheModeWriteCombined: MTLResourceOptions

This constant was deprecated in iOS 9.0 and macOS 10.11.

Deprecated

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Common Resource Functionality

protocol MTLAllocation

A memory allocation from a Metal GPU device, such as a memory heap, texture, or data buffer.

protocol MTLResource

An allocation of memory accessible to a GPU.

struct MTLResourceUsage

Options that describe how a graphics or compute function uses an argument buffer’s resource.

struct MTLResourceID

