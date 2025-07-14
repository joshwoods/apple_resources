

- Spatial
-  Rotatable3D 

Protocol

# Rotatable3D

A set of methods that defines the interface to rotate Spatial entities.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
protocol Rotatable3D
```

## Topics

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

func rotated(by: Rotation3D) -> Self

Returns the entity that results from applying the specified rotation.

**Required**

## Relationships

### Conforming Types

- AffineTransform3D
- Point3D
- Pose3D
- ProjectiveTransform3D
- Ray3D
- Rect3D
- Rotation3D
- ScaledPose3D
- Size3D
- Vector3D

## See Also

### Protocols

protocol Primitive3D

A set of methods common to Spatial primitives.

protocol Scalable3D

A set of methods that defines the interface to scale Spatial entities.

protocol Shearable3D

A set of methods that defines the interface to shear Spatial entities.

protocol Translatable3D

A set of methods that defines the interface to translate Spatial entities.

protocol Volumetric

A set of methods for working with Spatial primitives with volume.

