

- Core Animation
-  Transforms 

API Collection

# Transforms

Define transform matrices to apply affine transformations to layers in Core Animation.

## Topics

### Creating Transforms

func CATransform3DMakeTranslation(CGFloat, CGFloat, CGFloat) -> CATransform3D

Returns a transform that translates by `(tx, ty, tz)`.

func CATransform3DMakeScale(CGFloat, CGFloat, CGFloat) -> CATransform3D

Returns a transform that scales by `(sx, sy, sz)`.

func CATransform3DMakeRotation(CGFloat, CGFloat, CGFloat, CGFloat) -> CATransform3D

Returns a transform that rotates by `angle` radians about the vector `(x, y, z)`.

### Chaining Transforms

func CATransform3DConcat(CATransform3D, CATransform3D) -> CATransform3D

Concatenates `b` to `a` and returns the result: `t = a * b`.

func CATransform3DTranslate(CATransform3D, CGFloat, CGFloat, CGFloat) -> CATransform3D

Translates `t` by `(tx, ty, tz)` and returns the result: `t` `= translate(tx, ty, tz) * t`.

func CATransform3DScale(CATransform3D, CGFloat, CGFloat, CGFloat) -> CATransform3D

Scales `t` by `(sx, sy, sz)` and returns the result: `t = scale(sx, sy, sz) * t`.

func CATransform3DRotate(CATransform3D, CGFloat, CGFloat, CGFloat, CGFloat) -> CATransform3D

Rotates `t` by `angle` radians about the vector `(x, y, z)` and returns the result.

### Inverting a Transform

func CATransform3DInvert(CATransform3D) -> CATransform3D

Inverts `t` and returns the result.

### Determining Transform Properties

func CATransform3DIsAffine(CATransform3D) -> Bool

Returns a Boolean value that indicates whether a transform can be exactly represented by an affine transform.

func CATransform3DIsIdentity(CATransform3D) -> Bool

Returns a Boolean value that indicates whether the transform is the identity transform.

func CATransform3DEqualToTransform(CATransform3D, CATransform3D) -> Bool

Returns a Boolean value that indicates whether the two transforms are exactly equal.

### Converting to and from Core Graphics Affine Transforms

func CATransform3DMakeAffineTransform(CGAffineTransform) -> CATransform3D

Returns a transform with the same effect as affine transform `m`.

func CATransform3DGetAffineTransform(CATransform3D) -> CGAffineTransform

Returns the affine transform represented by `t`.

### Data Types

struct CATransform3D

The standard transform matrix used throughout Core Animation.

### Constants

let CATransform3DIdentity: CATransform3D

The identity transform: `[1 0 0 0; 0 1 0 0; 0 0 1 0; 0 0 0 1]`.

