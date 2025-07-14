

- Model I/O
- MDLVoxelArray
-  difference(with:) 

Instance Method

# difference(with:)

Reduces the voxel array to cover only the portion of its volume not covered by another voxel array.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func difference(with voxels: MDLVoxelArray)
```

## Parameters 

`voxels`  

The voxel array to subtract from this voxel array.

## Discussion

After a difference operation, the voxel array contains only those voxels that were present in the original array and not present in the specified array. That is, a difference operation creates a voxel array representing the space where one volume does not overlap another.

Performing a union, intersection, or difference operation clears out shell level information from all voxels in the array. (That is, the w component of every MDLVoxelIndex value in the voxel array is reset to 0.)

## See Also

### Performing Constructive Solid Geometry Operations

func union(with: MDLVoxelArray)

Extends the voxel array to also cover the volume of the specified voxel array.

func intersect(with: MDLVoxelArray)

Reduces the voxel array to cover only the volume within both it and another voxel array.

