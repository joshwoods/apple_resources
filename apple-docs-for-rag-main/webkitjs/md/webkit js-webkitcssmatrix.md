

- WebKit JS
-  WebKitCSSMatrix 

Class

# WebKitCSSMatrix

`WebKitCSSMatrix` objects represent a 4x4 homogeneous matrix for 3D transforms or a vector for 2D transforms. You can use these objects to manipulate matrices in JavaScript. For example, you can multiply, translate, and scale matrices.

Safari Desktop 10.0+Safari Mobile 2.0+

``` source
interface WebKitCSSMatrix
```

## Overview

The values of a 3D matrix can be initialized from the matrix3d transform function returned by `window.getComputedStyle(element).webkitTransform()`. To apply the final matrix to an element, construct a string using the matrix3d transform function passing the 16 values, and assign it to `element.style.webkitTransform`. Similarly, you can construct a matrix for 2D transforms by setting 6 values, represented by the `a`-`f` properties.

## Topics

### Accessing Properties

a

The first 2D vector value.

b

The second 2D vector value.

c

The third 2D vector value.

d

The fourth 2D vector value.

e

The fifth 2D vector value.

f

The sixth 2D vector value.

m11

The 3D matrix value in the first row and first column.

m12

The 3D matrix value in the first row and second column.

m13

The 3D matrix value in the first row and third column.

m14

The 3D matrix value in the first row and fourth column.

m21

The 3D matrix value in the second row and first column.

m22

The 3D matrix value in the second row and second column.

m23

The 3D matrix value in the second row and third column.

m24

The 3D matrix value in the second row and fourth column.

m31

The 3D matrix value in the third row and first column.

m32

The 3D matrix value in the third row and second column.

m33

The 3D matrix value in the third row and third column.

m34

The 3D matrix value in the third row and fourth column.

m41

The 3D matrix value in the fourth row and first column.

m42

The 3D matrix value in the fourth row and second column.

m43

The 3D matrix value in the fourth row and third column.

m44

The 3D matrix value in the fourth row and fourth column.

### Setting the Matrix

setMatrixValue

Sets the matrix values using a string representation.

### Applying Operations

multiply

Returns the result of multiplying this matrix by a given matrix that is on the right.

inverse

Returns the inverse of this matrix.

translate

Returns the result of translating this matrix by a given vector.

scale

Returns the result of scaling this matrix by a given vector.

rotate

Returns the result of rotating this matrix by a given vector.

rotateAxisAngle

Returns the result of rotating this matrix by a given vector and angle.

skewX

Specifies a skew transformation along the x-axis by the given angle.

skewY

Specifies a skew transformation along the y-axis by the given angle.

### Converting the Matrix

toString

Returns a string representation of the matrix.

