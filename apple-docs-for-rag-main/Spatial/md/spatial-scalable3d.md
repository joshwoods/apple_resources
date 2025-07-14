

- Spatial
-  Scalable3D 

Protocol

# Scalable3D

A set of methods that defines the interface to scale Spatial entities.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
protocol Scalable3D
```

## Topics

### Instance methods

func scale(by: Size3D)

Scales the entity by the specified size.

**Required** Default implementation provided.

func scaleBy(x: Double, y: Double, z: Double)

Scales the entity by the specified values.

**Required** Default implementation provided.

func scaled(by: Size3D) -> Self

Returns the entity that results from scaling with the specified size.

**Required**

func scaledBy(x: Double, y: Double, z: Double) -> Self

Returns the entity that results from scaling with the specified values.

**Required**

func uniformlyScale(by: Double)

Uniformly scales the entity by the specified scalar value.

**Required** Default implementation provided.

func uniformlyScaled(by: Double) -> Self

Returns the entity that results from uniformly scaling with the specified scalar value.

**Required**

## Relationships

### Conforming Types

- AffineTransform3D
- ProjectiveTransform3D
- Rect3D
- Size3D
- Vector3D

## See Also

### Protocols

protocol Primitive3D

A set of methods common to Spatial primitives.

protocol Rotatable3D

A set of methods that defines the interface to rotate Spatial entities.

protocol Shearable3D

A set of methods that defines the interface to shear Spatial entities.

protocol Translatable3D

A set of methods that defines the interface to translate Spatial entities.

protocol Volumetric

A set of methods for working with Spatial primitives with volume.

