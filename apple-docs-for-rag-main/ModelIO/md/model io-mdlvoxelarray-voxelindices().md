

- Model I/O
- MDLVoxelArray
-  voxelIndices() 

Instance Method

# voxelIndices()

Returns a data object containing all voxels within the voxel array.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func voxelIndices() -> Data?
```

## Return Value

A data object containing MDLVoxelIndex values.

## Discussion

The returned NSData object contains an array of MDLVoxelIndex values describing the locations of voxels within the voxel array as well as their volumetric relationship to the object modeled by the voxel array.

Calling this method is equivalent to calling the voxels(within:) method with the value of the voxelIndexExtent property.

## See Also

### Examining Voxels

var count: Int

The number of voxels in the array.

var voxelIndexExtent: MDLVoxelIndexExtent

The indexes that define the corners of the three-dimensional voxel grid.

func voxelExists(atIndex: MDLVoxelIndex, allowAnyX: Bool, allowAnyY: Bool, allowAnyZ: Bool, allowAnyShell: Bool) -> Bool

Returns a Boolean value indicating whether the voxel array contains voxel data for the specified index.

func voxels(within: MDLVoxelIndexExtent) -> Data?

Returns a data object containing all voxels within the specified volume.

