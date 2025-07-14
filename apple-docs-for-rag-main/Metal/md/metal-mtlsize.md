

- Metal
-  MTLSize 

Structure

# MTLSize

The dimensions of an object.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct MTLSize
```

## Mentioned in 

Converting Between Pixel Regions and Sparse Tile Regions

Creating a Rasterization Rate Map

Calculating Threadgroup and Grid Sizes

## Overview

Metal has many object types that represent arrays of discrete elements. For example, a texture has an array of pixel elements, and a thread grid has an array of computational threads. Use MTLSize instances to measure the extents of these objects or extents of regions within these objects.

Conceptually, when using a MTLSize instance to measure an object, treat the object as a 3D array of elements, even if it has fewer dimensions. Set the length of any unused dimensions to `1`. For example, a `5x5` 2D texture is a `5x5x1` texture in 3D.

## Topics

### Creating Sizes

init()

Initializes a box size.

init(width: Int, height: Int, depth: Int)

Initializes a size for an object with the specified dimensions.

func MTLSizeMake(Int, Int, Int) -> MTLSize

Creates a size for an object using the specified dimensions.

### Getting and Setting Dimensions

var width: Int

The number of elements in the x dimension.

var height: Int

The number of elements in the y dimension.

var depth: Int

The number of elements in the z dimension.

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

struct MTLOrigin

The coordinates for the front upper-left corner of a region.

struct MTLStageInRegionIndirectArguments

The data layout required for the arguments needed to specify the stage-in region.

struct MTLDispatchThreadgroupsIndirectArguments

The data layout required for arguments needed to specify the size of threadgroups.

