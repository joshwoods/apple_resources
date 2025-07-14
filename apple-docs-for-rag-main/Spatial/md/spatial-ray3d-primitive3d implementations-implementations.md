

- Spatial
- Ray3D
-  Primitive3D Implementations 

API Collection

# Primitive3D Implementations

## Topics

### Instance Properties

var isFinite: Bool

A Boolean value that indicates whether all of the values of the ray are finite.

var isNaN: Bool

A Boolean value that indicates whether the ray contains any NaN values.

var isZero: Bool

A Boolean value that indicates whether all of the values of the ray are zero.

### Instance Methods

func apply(Pose3D)

Applies the specified pose to the ray.

func applying(ProjectiveTransform3D) -> Ray3D

Returns a ray that results from applying the specified projective transform.

func applying(AffineTransform3D) -> Ray3D

Returns a ray that results from applying the specified affine transform.

func applying(Pose3D) -> Ray3D

Returns a ray that results from applying the specified pose.

func unapplying(ProjectiveTransform3D) -> Ray3D

Returns a ray that results from unapplying the specified projective transform.

func unapplying(AffineTransform3D) -> Ray3D

Returns a ray that results from unapplying the specified affine transform.

func unapplying(Pose3D) -> Ray3D

Unapplies the specified pose to the ray.

