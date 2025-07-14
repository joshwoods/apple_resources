

- Model I/O
- MDLVoxelArray
-  count 

Instance Property

# count

The number of voxels in the array.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var count: Int { get }
```

## Discussion

This property measures the number of grid positions in the array for which voxel data exists, not the total number of grid positions within the voxel array’s extent.

## See Also

### Examining Voxels

var voxelIndexExtent: MDLVoxelIndexExtent

The indexes that define the corners of the three-dimensional voxel grid.

func voxelExists(atIndex: MDLVoxelIndex, allowAnyX: Bool, allowAnyY: Bool, allowAnyZ: Bool, allowAnyShell: Bool) -> Bool

Returns a Boolean value indicating whether the voxel array contains voxel data for the specified index.

func voxels(within: MDLVoxelIndexExtent) -> Data?

Returns a data object containing all voxels within the specified volume.

func voxelIndices() -> Data?

Returns a data object containing all voxels within the voxel array.

