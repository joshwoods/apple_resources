

- PHASE
- PHASEObject
-  transform 

Instance Property

# transform

A matrix, in local coordinates, that determines the object’s pose in the scene.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var transform: simd_float4x4 { get set }
```

## Mentioned in 

Playing sound from a location in a 3D scene

## Discussion

The value of this property requires orthogonal basis vectors and uniform scale.

The framework interprets the transform’s position values in a right-handed coordinate system, where the *Y* axis extends upward and and the negative *Z* axis extends forward.

### Set an Object’s Position

An object positions in the 3D scene by the transformʼs first 3 elements of the last column. The following code sets an object’s position to `(0,0,-6)`, which is 6 meters in front of the world origin `(0,0,0)`.

```
var boardPieceTransform: simd_float4x4 = matrix_identity_float4x4
boardPieceTransform.columns.3.z -= 6.0
boardPieceSource.transform = boardPieceTransform
```

Set the unitsPerMeter parameter to instruct PHASE to interpret transform values in your app’s preferred unit of measurement.

## See Also

### Defining a Pose

var worldTransform: simd_float4x4

A matrix, in scene coordinates, that determines the object’s pose in the scene.

