

- Spatial
- Primitive3D
-  unapply(\_:) 

Instance Method

# unapply(\_:)

Unapplies an affine transform.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
mutating func unapply(_ transform: AffineTransform3D)
```

**Required** Default implementations provided.

## Parameters 

`transform`  

The affine transform that the function unapplies to the Spatial primitive.

## Default Implementations

### Primitive3D Implementations

func unapply(ProjectiveTransform3D)

Unapplies a projective transform.

func unapply(AffineTransform3D)

Unapplies an affine transform.

func unapply(Pose3D)

## See Also

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

