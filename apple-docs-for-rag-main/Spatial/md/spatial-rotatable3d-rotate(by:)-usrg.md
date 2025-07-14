

- Spatial
- Rotatable3D
-  rotate(by:) 

Instance Method

# rotate(by:)

Rotates the entity by a quaternion.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
mutating func rotate(by quaternion: simd_quatd)
```

**Required** Default implementations provided.

## Parameters 

`quaternion`  

The double-precision quaternion that specifies the rotation.

## Default Implementations

### Rotatable3D Implementations

func rotate(by: simd_quatd)

Rotates the entity by a quaternion.

func rotate(by: Rotation3D)

Rotates the entity by an angle over an axis.

## See Also

### Instance methods

func rotate(by: Rotation3D)

Rotates the entity by an angle over an axis.

**Required** Default implementations provided.

func rotated(by: simd_quatd) -> Self

Returns the entity that a quaternion rotates.

**Required**

func rotated(by: Rotation3D) -> Self

Returns the entity that results from applying the specified rotation.

**Required**

