

- Model I/O
-  MDLVoxelIndex 

Type Alias

# MDLVoxelIndex

A 4-component vector encoding the location of a voxel in a voxel array and describing its relation to an object’s volume.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
typealias MDLVoxelIndex = vector_int4
```

## Discussion

A voxel index provides both location and description information for a voxel:

- The x, y, and z components provide the absolute location of the voxel within the three-dimensional grid of a voxel array, as bounded by the voxel array’s voxelIndexExtent property.

- The w component is the shell index for the voxel, describing its location relative to the volume of the object the voxel array represents. A shell index of zero means the voxel is on the surface of an object. Positive shell indices indicate voxels outside of the object’s surface, and negative shell indices lie inside of the object. Increments of shell index correspond to concentric shells, nested within each other inside the object or enclosing one another outside of the object.

## See Also

### Constants

struct MDLVoxelIndexExtent

The corner voxel indices defining a solid rectangular volume of voxels. Used by the voxelIndexExtent property and voxels(within:) method.

