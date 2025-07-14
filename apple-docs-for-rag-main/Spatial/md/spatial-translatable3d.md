

- Spatial
-  Translatable3D 

Protocol

# Translatable3D

A set of methods that defines the interface to translate Spatial entities.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
protocol Translatable3D
```

## Topics

### Instance methods

func translate(by: Vector3D)

Translates the entity by the specified vector.

**Required** Default implementations provided.

func translated(by: Vector3D) -> Self

Returns the entity that results from translating with the specified vector.

**Required** Default implementation provided.

### Deprecated methods

func translate(by: Size3D)

Translates the entity by the specified size.

**Required** Default implementations provided.

Deprecated

func translated(by: Size3D) -> Self

Returns the entity that results from translating with the specified size.

**Required** Default implementation provided.

Deprecated

## Relationships

### Conforming Types

- AffineTransform3D
- Point3D
- Pose3D
- ProjectiveTransform3D
- Ray3D
- Rect3D
- ScaledPose3D

## See Also

### Protocols

protocol Primitive3D

A set of methods common to Spatial primitives.

protocol Rotatable3D

A set of methods that defines the interface to rotate Spatial entities.

protocol Scalable3D

A set of methods that defines the interface to scale Spatial entities.

protocol Shearable3D

A set of methods that defines the interface to shear Spatial entities.

protocol Volumetric

A set of methods for working with Spatial primitives with volume.

