

- Spatial
- Primitive3D
-  apply(\_:) 

Instance Method

# apply(\_:)

Applies a pose.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
mutating func apply(_ pose: Pose3D)
```

**Required** Default implementations provided.

## Parameters 

`pose`  

The pose that the function applies to the Spatial primitive.

## Default Implementations

### Primitive3D Implementations

func apply(Pose3D)

func apply(AffineTransform3D)

Applies an affine transform.

func apply(ProjectiveTransform3D)

Applies a projective transform.

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

