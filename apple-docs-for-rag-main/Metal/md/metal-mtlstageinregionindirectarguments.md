

- Metal
-  MTLStageInRegionIndirectArguments 

Structure

# MTLStageInRegionIndirectArguments

The data layout required for the arguments needed to specify the stage-in region.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
struct MTLStageInRegionIndirectArguments
```

## Topics

### Initializers

init()

init(stageInOrigin: (UInt32, UInt32, UInt32), stageInSize: (UInt32, UInt32, UInt32))

### Instance Properties

var stageInOrigin: (UInt32, UInt32, UInt32)

The location of the upper-left corner of the block.

var stageInSize: (UInt32, UInt32, UInt32)

The size of the block.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Indirect Compute Commands

protocol MTLIndirectComputeCommand

A compute command in an indirect command buffer.

struct MTLRegion

The bounds for a subset of an object’s elements.

struct MTLSize

The dimensions of an object.

struct MTLOrigin

The coordinates for the front upper-left corner of a region.

struct MTLDispatchThreadgroupsIndirectArguments

The data layout required for arguments needed to specify the size of threadgroups.

