

- Spatial
- Primitive3D
-  unapplying(\_:) 

Instance Method

# unapplying(\_:)

Returns the entity that results from unapplying a projective transform.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func unapplying(_ transform: ProjectiveTransform3D) -> Self
```

**Required**

## Parameters 

`transform`  

The projective transform that the function unapplies to the Spatial primitive.

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

func unapply(AffineTransform3D)

Unapplies an affine transform.

**Required** Default implementations provided.

func unapply(ProjectiveTransform3D)

Unapplies a projective transform.

**Required** Default implementations provided.

func unapplying(AffineTransform3D) -> Self

Returns the entity that results from unapplying an affine transform.

**Required**

func unapply(Pose3D)

Unapplies a pose.

**Required** Default implementations provided.

func unapplying(Pose3D) -> Self

Returns the entity that results from unapplying a pose.

**Required**

