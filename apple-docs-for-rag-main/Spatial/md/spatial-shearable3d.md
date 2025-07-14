

- Spatial
-  Shearable3D 

Protocol

# Shearable3D

A set of methods that defines the interface to shear Spatial entities.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
protocol Shearable3D
```

## Topics

### Instance methods

func shear(AxisWithFactors)

Shears the entity by the specified axis and shear factors.

**Required** Default implementation provided.

func sheared(AxisWithFactors) -> Self

Returns the entity that results from shearing with the specified axis and shear factors.

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

protocol Scalable3D

A set of methods that defines the interface to scale Spatial entities.

protocol Translatable3D

A set of methods that defines the interface to translate Spatial entities.

protocol Volumetric

A set of methods for working with Spatial primitives with volume.

