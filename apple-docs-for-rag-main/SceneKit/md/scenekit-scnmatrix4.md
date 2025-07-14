

- SceneKit
-  SCNMatrix4 

Type Alias

# SCNMatrix4

A representation of a 4 x 4 matrix.

macOS

``` source
typealias SCNMatrix4 = CATransform3D
```

## Discussion

SceneKit uses matrices to represent coordinate space transformations, which in turn can represent the combined position, rotation or orientation, and scale of an object in three-dimensional space.

Important

In macOS, the fields in this structure are CGFloat values. In iOS, tvOS, and watchOS, these fields are `float` values.

## Topics

### Creating Transform Matrices

func SCNMatrix4MakeTranslation(Float, Float, Float) -> SCNMatrix4

Returns a matrix describing a translation transformation.

func SCNMatrix4MakeRotation(Float, Float, Float, Float) -> SCNMatrix4

Returns a matrix describing a rotation transformation.

func SCNMatrix4MakeScale(Float, Float, Float) -> SCNMatrix4

Returns a matrix describing a scale transformation.

### Performing Matrix Operations

func SCNMatrix4Translate(SCNMatrix4, Float, Float, Float) -> SCNMatrix4

Returns a new matrix created by concatenating the specified matrix with a translation transformation.

func SCNMatrix4Rotate(SCNMatrix4, Float, Float, Float, Float) -> SCNMatrix4

Returns a new matrix created by concatenating the specified matrix with a rotation transformation.

func SCNMatrix4Scale(SCNMatrix4, Float, Float, Float) -> SCNMatrix4

Returns a new matrix created by concatenating the specified matrix with a scale transformation.

func SCNMatrix4Invert(SCNMatrix4) -> SCNMatrix4

Returns the inverse of the specified matrix.

func SCNMatrix4Mult(SCNMatrix4, SCNMatrix4) -> SCNMatrix4

Returns the product of two matrices.

### Converting Matrix Types

func SCNMatrix4FromGLKMatrix4(GLKMatrix4) -> SCNMatrix4

Returns a SceneKit matrix corresponding to a GLKit matrix.

func SCNMatrix4ToGLKMatrix4(SCNMatrix4) -> GLKMatrix4

Returns a GLKit matrix corresponding to a SceneKit matrix.

### Comparing Matrices

func SCNMatrix4EqualToMatrix4(SCNMatrix4, SCNMatrix4) -> Bool

Returns a Boolean value that indicates whether the corresponding elements of two matrices are equal.

func SCNMatrix4IsIdentity(SCNMatrix4) -> Bool

Returns a Boolean value that indicates whether the specified matrix is equal to the identity matrix.

### Identity Constant

let SCNMatrix4Identity: SCNMatrix4

The 4 x 4 identity matrix.

### Matrix Elements

var m11: Float

var m12: Float

var m13: Float

var m14: Float

var m21: Float

var m22: Float

var m23: Float

var m24: Float

var m31: Float

var m32: Float

var m33: Float

var m34: Float

var m41: Float

var m42: Float

var m43: Float

var m44: Float

## See Also

### Transforms and Rotations

struct SCNMatrix4

A representation of a 4 x 4 matrix.

typealias SCNQuaternion

A representation of a quaternion.

