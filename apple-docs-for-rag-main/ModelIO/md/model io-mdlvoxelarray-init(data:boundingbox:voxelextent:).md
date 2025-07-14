

- Model I/O
- MDLVoxelArray
-  init(data:boundingBox:voxelExtent:) 

Initializer

# init(data:boundingBox:voxelExtent:)

Initializes a voxel array with the specified voxel data.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
init(
    data voxelData: Data,
    boundingBox: MDLAxisAlignedBoundingBox,
    voxelExtent: Float
)
```

## Parameters 

`voxelData`  

A data object containing an array of MDLVoxelIndex values, each of which describes the locations of voxels within the specified volume as well as their volumetric relationship to the object modeled by the voxel array.

`boundingBox`  

The extent of the voxel array’s volume in world coordinate space.

`voxelExtent`  

The size of a single voxel in world coordinate space.

## Return Value

A new voxel array.

## Discussion

The `boundingBox` parameter relates the integer grid of the newly created voxel array to a continuous Cartesian space. The methods listed in Relating Voxels to Scene Space and Creating a Mesh from Voxels operate with respect to this bounding volume.

## See Also

### Creating a Voxel Array

init(asset: MDLAsset, divisions: Int32, interiorShells: Int32, exteriorShells: Int32, patchRadius: Float)

Initializes a voxel array that models the volume of 3D objects in the specified asset and creates the specified number of voxel shells.

Deprecated

init(asset: MDLAsset, divisions: Int32, interiorNBWidth: Float, exteriorNBWidth: Float, patchRadius: Float)

Initializes a voxel array that models the volume of 3D objects in the specified asset, creating voxel shells for the specified distances from the object’s surface.

Deprecated

