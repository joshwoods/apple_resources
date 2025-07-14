

- Spatial
-  Primitive3D 

Protocol

# Primitive3D

A set of methods common to Spatial primitives.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
protocol Primitive3D : Decodable, Encodable, Equatable
```

## Topics

### Instance properties

var isFinite: Bool

Returns a Boolean value that indicates whether the primitive is infinite.

**Required**

var isNaN: Bool

Returns a Boolean value that indicates whether the primitive contains any NaN values.

**Required**

var isZero: Bool

Returns a Boolean value that indicates whether the primitive is zero.

**Required**

### Type properties

static var infinity: Self

A primitive with infinite values.

**Required**

static var zero: Self

A primitive with zero values.

**Required**

### Transforming primitives

func apply(AffineTransform3D)

Applies an affine transform.

**Required** Default implementations provided.

func apply(ProjectiveTransform3D)

Applies a projective transform.

**Required** Default implementations provided.

func applying(AffineTransform3D) -> Self

Returns the entity that results from applying an affine transform.

**Required**

func applying(ProjectiveTransform3D) -> Self

Returns the entity that results from applying a projective transform.

**Required**

func apply(Pose3D)

Applies a pose.

**Required** Default implementations provided.

func applying(Pose3D) -> Self

Returns the entity that results from applying a pose.

**Required**

func unapply(AffineTransform3D)

Unapplies an affine transform.

**Required** Default implementations provided.

func unapply(ProjectiveTransform3D)

Unapplies a projective transform.

**Required** Default implementations provided.

func unapplying(AffineTransform3D) -> Self

Returns the entity that results from unapplying an affine transform.

**Required**

func unapplying(ProjectiveTransform3D) -> Self

Returns the entity that results from unapplying a projective transform.

**Required**

func unapply(Pose3D)

Unapplies a pose.

**Required** Default implementations provided.

func unapplying(Pose3D) -> Self

Returns the entity that results from unapplying a pose.

**Required**

## Relationships

### Inherits From

- Decodable
- Encodable
- Equatable

### Conforming Types

- Point3D
- Ray3D
- Rect3D
- Size3D
- Vector3D

## See Also

### Protocols

protocol Rotatable3D

A set of methods that defines the interface to rotate Spatial entities.

protocol Scalable3D

A set of methods that defines the interface to scale Spatial entities.

protocol Shearable3D

A set of methods that defines the interface to shear Spatial entities.

protocol Translatable3D

A set of methods that defines the interface to translate Spatial entities.

protocol Volumetric

A set of methods for working with Spatial primitives with volume.

