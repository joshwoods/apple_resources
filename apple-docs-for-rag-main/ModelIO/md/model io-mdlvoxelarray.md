

- Model I/O
-  MDLVoxelArray 

Class

# MDLVoxelArray

A model of a 3D object’s solid volume as a collection of *voxels*, or cubic units.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class MDLVoxelArray
```

## Overview

Unlike a mesh, which models only surface topology, a voxel array models the solid volume of a 3D object. Voxels are useful for modeling volumetric phenomena (such as clouds and fire), performing solid geometry operations (such as intersection and union), and preparing a 3D design for real-world physical production.

## Topics

### Creating a Voxel Array

init(asset: MDLAsset, divisions: Int32, interiorShells: Int32, exteriorShells: Int32, patchRadius: Float)

Initializes a voxel array that models the volume of 3D objects in the specified asset and creates the specified number of voxel shells.

Deprecated

init(asset: MDLAsset, divisions: Int32, interiorNBWidth: Float, exteriorNBWidth: Float, patchRadius: Float)

Initializes a voxel array that models the volume of 3D objects in the specified asset, creating voxel shells for the specified distances from the object’s surface.

Deprecated

init(data: Data, boundingBox: MDLAxisAlignedBoundingBox, voxelExtent: Float)

Initializes a voxel array with the specified voxel data.

### Examining Voxels

var count: Int

The number of voxels in the array.

var voxelIndexExtent: MDLVoxelIndexExtent

The indexes that define the corners of the three-dimensional voxel grid.

func voxelExists(atIndex: MDLVoxelIndex, allowAnyX: Bool, allowAnyY: Bool, allowAnyZ: Bool, allowAnyShell: Bool) -> Bool

Returns a Boolean value indicating whether the voxel array contains voxel data for the specified index.

func voxels(within: MDLVoxelIndexExtent) -> Data?

Returns a data object containing all voxels within the specified volume.

func voxelIndices() -> Data?

Returns a data object containing all voxels within the voxel array.

### Modifying Voxels

func setVoxelAtIndex(MDLVoxelIndex)

Sets voxel characteristics at the specified index in the array.

func setVoxelsFor(MDLMesh, divisions: Int32, interiorNBWidth: Float, exteriorNBWidth: Float, patchRadius: Float)

Sets voxel values in the array to model the volume of the specified mesh and creates voxel shells for the specified distances from the object’s surface.

Deprecated

func setVoxelsFor(MDLMesh, divisions: Int32, interiorShells: Int32, exteriorShells: Int32, patchRadius: Float)

Sets voxel values in the array to model the volume of the specified mesh and creates the specified number of voxel shells.

Deprecated

### Performing Constructive Solid Geometry Operations

func union(with: MDLVoxelArray)

Extends the voxel array to also cover the volume of the specified voxel array.

func intersect(with: MDLVoxelArray)

Reduces the voxel array to cover only the volume within both it and another voxel array.

func difference(with: MDLVoxelArray)

Reduces the voxel array to cover only the portion of its volume not covered by another voxel array.

### Relating Voxels to Scene Space

var boundingBox: MDLAxisAlignedBoundingBox

The extent of the voxel array’s volume in world coordinate space.

func index(ofSpatialLocation: vector_float3) -> MDLVoxelIndex

Returns voxel information corresponding to the specified point in the world coordinate space of the asset from which the voxel array was created.

func spatialLocation(ofIndex: MDLVoxelIndex) -> vector_float3

Returns the location of the specified voxel in world coordinate space.

func voxelBoundingBox(atIndex: MDLVoxelIndex) -> MDLAxisAlignedBoundingBox

Returns the extent of the specified voxel’s volume in the world coordinate space of the asset from which the voxel array was created.

### Creating a Mesh from Voxels

func mesh(using: (any MDLMeshBufferAllocator)?) -> MDLMesh?

Generates a closed polygon mesh around the volume of space the voxel array describes.

### Constants

typealias MDLVoxelIndex

A 4-component vector encoding the location of a voxel in a voxel array and describing its relation to an object’s volume.

struct MDLVoxelIndexExtent

The corner voxel indices defining a solid rectangular volume of voxels. Used by the voxelIndexExtent property and voxels(within:) method.

### Initializers

init(asset: MDLAsset, divisions: Int32, patchRadius: Float)

### Instance Properties

var isValidSignedShellField: Bool

var shellFieldExteriorThickness: Float

var shellFieldInteriorThickness: Float

### Instance Methods

func coarseMesh() -> MDLMesh?

func coarseMesh(using: (any MDLMeshBufferAllocator)?) -> MDLMesh?

func convertToSignedShellField()

func setVoxelsFor(MDLMesh, divisions: Int32, patchRadius: Float)

## Relationships

### Inherits From

- MDLObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- MDLNamed
- NSObjectProtocol

