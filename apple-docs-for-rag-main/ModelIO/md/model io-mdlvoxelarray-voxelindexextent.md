

- Model I/O
- MDLVoxelArray
-  voxelIndexExtent 

Instance Property

# voxelIndexExtent

The indexes that define the corners of the three-dimensional voxel grid.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var voxelIndexExtent: MDLVoxelIndexExtent { get }
```

## Discussion

This property determines which MDLVoxelIndex values are valid for referring to the contents of the voxel array using methods such as setVoxelAtIndex(_:) or voxelBoundingBox(atIndex:). For example, if the minimum extent is `{0, 0, 0, 0}` and the maximum extent is `{10, 10, 10, 0}`, the voxel index `{5, 5, 5, 0}` lies within the array but the voxel index `{0, 20, 10, 0}` does not.

## See Also

### Examining Voxels

var count: Int

The number of voxels in the array.

func voxelExists(atIndex: MDLVoxelIndex, allowAnyX: Bool, allowAnyY: Bool, allowAnyZ: Bool, allowAnyShell: Bool) -> Bool

Returns a Boolean value indicating whether the voxel array contains voxel data for the specified index.

func voxels(within: MDLVoxelIndexExtent) -> Data?

Returns a data object containing all voxels within the specified volume.

func voxelIndices() -> Data?

Returns a data object containing all voxels within the voxel array.

