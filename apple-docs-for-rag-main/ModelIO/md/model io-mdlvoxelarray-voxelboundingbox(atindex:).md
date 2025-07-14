

- Model I/O
- MDLVoxelArray
-  voxelBoundingBox(atIndex:) 

Instance Method

# voxelBoundingBox(atIndex:)

Returns the extent of the specified voxel’s volume in the world coordinate space of the asset from which the voxel array was created.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func voxelBoundingBox(atIndex index: MDLVoxelIndex) -> MDLAxisAlignedBoundingBox
```

## Parameters 

`index`  

An index describing the location of a voxel within the three-dimensional grid of the voxel array. (The w component is ignored for this query.)

## Return Value

The bounding box for the single voxel at the specified index, in the world coordinate space of the asset from which the voxel array was created.

## Discussion

The coordinate space for spatial locations of voxels is the world space of the asset from which the voxel array was created, or for voxel arrays created with the init(data:boundingBox:voxelExtent:) initializer, the bounding box specified at initialization.

## See Also

### Relating Voxels to Scene Space

var boundingBox: MDLAxisAlignedBoundingBox

The extent of the voxel array’s volume in world coordinate space.

func index(ofSpatialLocation: vector_float3) -> MDLVoxelIndex

Returns voxel information corresponding to the specified point in the world coordinate space of the asset from which the voxel array was created.

func spatialLocation(ofIndex: MDLVoxelIndex) -> vector_float3

Returns the location of the specified voxel in world coordinate space.

