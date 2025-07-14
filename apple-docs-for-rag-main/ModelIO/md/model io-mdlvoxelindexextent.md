

- Model I/O
-  MDLVoxelIndexExtent 

Structure

# MDLVoxelIndexExtent

The corner voxel indices defining a solid rectangular volume of voxels. Used by the voxelIndexExtent property and voxels(within:) method.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
struct MDLVoxelIndexExtent
```

## Topics

### Initializers

init()

init(minimumExtent: MDLVoxelIndex, maximumExtent: MDLVoxelIndex)

### Instance Properties

var maximumExtent: MDLVoxelIndex

The highest x, y, and z coordinates in the volume.

var minimumExtent: MDLVoxelIndex

The lowest x, y, and z coordinates in the volume.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Constants

typealias MDLVoxelIndex

A 4-component vector encoding the location of a voxel in a voxel array and describing its relation to an object’s volume.

