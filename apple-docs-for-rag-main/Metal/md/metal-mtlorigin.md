

- Metal
-  MTLOrigin 

Structure

# MTLOrigin

The coordinates for the front upper-left corner of a region.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct MTLOrigin
```

## Topics

### Creating Origin Points

init()

Initializes a new origin.

init(x: Int, y: Int, z: Int)

Initializes a new origin with the specified coordinates.

func MTLOriginMake(Int, Int, Int) -> MTLOrigin

Returns a new origin with the specified coordinates.

### Getting and Setting Coordinate Values

var x: Int

The x coordinate of the origin.

var y: Int

The y coordinate of the origin.

var z: Int

The z coordinate of the origin.

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

struct MTLStageInRegionIndirectArguments

The data layout required for the arguments needed to specify the stage-in region.

struct MTLDispatchThreadgroupsIndirectArguments

The data layout required for arguments needed to specify the size of threadgroups.

