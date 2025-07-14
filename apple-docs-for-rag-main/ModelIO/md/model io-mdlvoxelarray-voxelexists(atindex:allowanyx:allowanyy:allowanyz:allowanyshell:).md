

- Model I/O
- MDLVoxelArray
-  voxelExists(atIndex:allowAnyX:allowAnyY:allowAnyZ:allowAnyShell:) 

Instance Method

# voxelExists(atIndex:allowAnyX:allowAnyY:allowAnyZ:allowAnyShell:)

Returns a Boolean value indicating whether the voxel array contains voxel data for the specified index.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func voxelExists(
    atIndex index: MDLVoxelIndex,
    allowAnyX: Bool,
    allowAnyY: Bool,
    allowAnyZ: Bool,
    allowAnyShell: Bool
) -> Bool
```

## Parameters 

`index`  

An index describing both the location of the voxel within the three-dimensional grid of the voxel array and its relationship to the volume of the object modeled by the voxel array.

`allowAnyX`  

If true, this method treats the x component of the index parameter as a wildcard. If false, this method requires an exact match for the x component.

`allowAnyY`  

If true, this method treats the y component of the index parameter as a wildcard. If false, this method requires an exact match for the y component.

`allowAnyZ`  

If true, this method treats the z component of the index parameter as a wildcard. If false, this method requires an exact match for the z component.

`allowAnyShell`  

If true, this method treats the w (shell level) component of the index parameter as a wildcard. If false, this method requires an exact match for the shell level component.

## Return Value

true if the voxel array contains at least one voxel index matching the specified parameters; otherwise false.

## Discussion

Use the `allowAnyX`, `allowAnyY`, `allowAnyZ`, and `allowAnyShell` parameters to perform wildcard searches. For example:

- Swift
- Objective-C

```
// Does a voxel exist at exactly the specified X, Y, Z, and shell level?
exists = voxelArray.voxelExists(atIndex: index, allowAnyX: false, allowAnyY: false, allowAnyZ: false, allowAnyShell: false)
// Does a voxel exist at the specified X, Y, and Z, regardless of shell level?
exists = voxelArray.voxelExists(atIndex: index, allowAnyX: false, allowAnyY: false, allowAnyZ: false, allowAnyShell: true)
// Are there surface voxels anywhere on the XY plane at a specific Z index?
index.w = 0
exists = voxelArray.voxelExists(atIndex: index, allowAnyX: true, allowAnyY: true, allowAnyZ: false, allowAnyShell: false)
// Are there any voxels three layers deep inside the object modeled by the voxel array, regardless of location?
index.w = -3
exists = voxelArray.voxelExists(atIndex: index, allowAnyX: true, allowAnyY: true, allowAnyZ: true, allowAnyShell: false)
```

```
// Does a voxel exist at exactly the specified X, Y, Z, and shell level?
exists = [voxelArray voxelExistsAtIndex:index allowAnyX:NO allowAnyY:NO allowAnyZ:NO allowAnyShell:NO];
// Does a voxel exist at the specified X, Y, and Z, regardless of shell level?
exists = [voxelArray voxelExistsAtIndex:index allowAnyX:NO allowAnyY:NO allowAnyZ:NO allowAnyShell:YES];
// Are there surface voxels anywhere on the XY plane at a specific Z index?
index.w = 0;
exists = [voxelArray voxelExistsAtIndex:index allowAnyX:YES allowAnyY:YES allowAnyZ:NO allowAnyShell:NO];
// Are there any voxels three layers deep inside the object modeled by the voxel array, regardless of location?
index.w = -3;
exists = [voxelArray voxelExistsAtIndex:index allowAnyX:YES allowAnyY:YES allowAnyZ:YES allowAnyShell:NO];
```

## See Also

### Examining Voxels

var count: Int

The number of voxels in the array.

var voxelIndexExtent: MDLVoxelIndexExtent

The indexes that define the corners of the three-dimensional voxel grid.

func voxels(within: MDLVoxelIndexExtent) -> Data?

Returns a data object containing all voxels within the specified volume.

func voxelIndices() -> Data?

Returns a data object containing all voxels within the voxel array.

