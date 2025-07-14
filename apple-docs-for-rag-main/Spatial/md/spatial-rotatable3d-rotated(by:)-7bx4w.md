

- Spatial
- Rotatable3D
-  rotated(by:) 

Instance Method

# rotated(by:)

Returns the entity that results from applying the specified rotation.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func rotated(by rotation: Rotation3D) -> Self
```

**Required**

## Parameters 

`rotation`  

The rotation structure that defines the rotation’s angle and axis.

## See Also

### Instance methods

func rotate(by: simd_quatd)

Rotates the entity by a quaternion.

**Required** Default implementations provided.

func rotate(by: Rotation3D)

Rotates the entity by an angle over an axis.

**Required** Default implementations provided.

func rotated(by: simd_quatd) -> Self

Returns the entity that a quaternion rotates.

**Required**

